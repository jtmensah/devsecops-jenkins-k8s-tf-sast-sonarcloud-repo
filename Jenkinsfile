pipeline {
  agent any
  tools { 
        maven 'Maven-Default'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=jm-devsecops_jm -Dsonar.organization=JM-Devsecops -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=c72fa8157921d2fc0cf0c597543320a4d8bda1b9'
			}
        } 
  }
}
