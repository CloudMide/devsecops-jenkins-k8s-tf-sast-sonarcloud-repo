pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asgbuggywebappmide -Dsonar.organization=asgbuggywebappmide -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=8ad2a2405c5cfcdd7639e2fe6326ac8b9f8b652b'
			}
        } 
  }
}
