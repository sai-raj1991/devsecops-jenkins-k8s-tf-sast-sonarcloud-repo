pipeline {
  agent any
  tools { 
        maven 'Maven_3_2_5'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asgbuggywebapp2035 -Dsonar.organization=sai -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=a9e1fc62e15258453142562b1fad1795e4892ed9'
			}
        } 
  }
}
