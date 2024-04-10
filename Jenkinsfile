pipeline {
  agent any
  tools { 
        maven 'Maven_3_2_5'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=jeffrey-buggy-webapp -Dsonar.organization=jeffrey-buggy-webapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=1cff6e854ef52abf02495b2ee5326579ce4d6847'
			}
        } 
  }
}
