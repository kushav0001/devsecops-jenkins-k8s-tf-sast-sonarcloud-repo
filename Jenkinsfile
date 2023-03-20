pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=kushavwebapp -Dsonar.organization=kushavwebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=4e1cc53d3ee9ac5ba2ad06f5ba42e4aae2600749'
			}
        } 
  }
}
