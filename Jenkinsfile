pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=jenkinssona -Dsonar.organization=jenkinssona -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=0f0ca0e6943290b7cc2221c071d1492e5f474261'
			}
        } 
  }
}
