pipeline {
  agent any
  tools { 
        maven 'Maven-Default'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=jm-devsecops_jm -Dsonar.organization=jm-devsecops -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=95979120b8a80dac31363d4c93425a0c40e05d7f'
			}
        } 
  }
}
