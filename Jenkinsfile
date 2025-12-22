pipeline {
  agent any
  tools { 
        maven 'Maven_3_8_4'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify org.sonarsource.scanner.maven:sonar-maven-plugin:sonar -Dsonar.projectKey=spidey48 -Dsonar.organization=spidey48 -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=97513d3309b3e8703cfa9fbdd0be6a2e8c63456e -Dsonar.javascript.enabled=false'
			}
        } 
  }
}
