pipeline {
  agent any
  tools { 
        maven "maven-3.5.2"  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asecurityguru -Dsonar.organization=asecurityguru -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=1ac5b857702589c6853cf5e066ac579f87e02c12'
			}
        } 
  }
}
