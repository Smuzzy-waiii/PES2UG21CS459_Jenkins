pipeline {
	agent any
	stages {
		stage('Build') {
			steps {
				build 'PES2UG21CS459-1'
				sh 'g++ main/hello.cpp -o output'
			}
		}
		stage('Test') {
			steps {
				sh './output'
			}
		}
		stage('Deploy') {
			steps {
				sg "./hghhhh"
			}
		}
	}
	post {
		failure{
			error 'Pipeline failure'
		}
	}
}