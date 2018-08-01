pipeline {
	agent any
	stages {
		stage ('Cleanup') {
			steps {
				deleteDir()
			}
		}
		
		stage ('Checkout SCM') {
			steps {
				checkout scm
			}
		}
		
		stage ('NPM install') {
			steps {
				sh '''cd test-app && npm install'''
			}
		}
	}
}
