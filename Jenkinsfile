pipeline {
	agent any
	stages {
		stage('ListFiles') {
			steps {
				sh 'ls'
			}
		}
	}
	post {
		always {
			echo "I just finished. Deleting the workspace now..."
			deleteDir()
		}
		failure {
			echo "I failed!"
		}
		success {
			echo "I completed successfully"
		}
		unstable {
			echo "I am in an unstable state"
		}
		changed {
			echo "Things were different before - something changed."
		}
	}
}
