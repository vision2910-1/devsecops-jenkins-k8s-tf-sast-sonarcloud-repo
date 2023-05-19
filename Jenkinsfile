pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=test-sonar-project1 -Dsonar.organization=test-sonal-project -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=5938c8c318176f5a13083562dfc8c06c18552477'
			}
        } 
  }
}
