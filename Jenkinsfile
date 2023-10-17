pipeline {
	agent any 
	tools {
		maven 'maven'
	}
	stages {
		stage('runsonarcloud') {
			steps {
				sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=buggy-webapp_a-buggy-webapp -Dsonar.organization=buggy-webapp -Dsonar.host.url=https://sonarcloud.io/ -Dsonar.login=65169cb11f9d60499e53a245b54c59af20394eb5'
				
			}
		}
	}
	
}
