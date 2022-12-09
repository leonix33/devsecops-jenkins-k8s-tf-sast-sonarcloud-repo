pipeline {
  agent any
  tools { 
        maven 'Maven 3.8.6'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=leonixpro -Dsonar.organization=leonixpro -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=3a98417867bc45d23f99c2c79bab7f2f27634d40'
			}
        } 
  }
}
