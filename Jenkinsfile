pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=DevSecOpsPankaj -Dsonar.organization=devsecopspankaj -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=a6060db575991a647e5d893ca47ccf3fbfdcaa31'
			}
        } 
  }
}
