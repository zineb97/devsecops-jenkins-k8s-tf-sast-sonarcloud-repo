pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asgbuggywebappz_asgbuggywebappz -Dsonar.organization=asgbuggywebappz -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=TOKEN'
			}
        } 
  }
}
