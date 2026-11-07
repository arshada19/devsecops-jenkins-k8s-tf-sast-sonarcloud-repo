pipeline {
  agent any
  tools { 
        maven 'Maven_3_8_4'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify org.sonarsource.scanner.maven:sonar-maven-plugin:sonar -Dsonar.projectKey=arshada -Dsonar.organization=arshada -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=66d44abbac63381b1d9158f95eb09abc5abf3165'
			}
        } 
  }
}
