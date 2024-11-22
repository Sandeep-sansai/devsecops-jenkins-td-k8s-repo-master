pipeline {
  agent any
  tools { 
        maven 'Maven_3_2_5'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=sandeep-sansai_newproject -Dsonar.organization=sandeep-sansai -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=75534ba5edeee7410074bdac4ec803ca357285d2'
			}
        } 
  }
}
