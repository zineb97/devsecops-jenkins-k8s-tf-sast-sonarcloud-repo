pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asgbuggywebappz_asgbuggywebappz -Dsonar.organization=asgbuggywebappz -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=6d27bef194d0bbf5ea5affddb6b36c7257439964'
			}
        } 
  }
}
