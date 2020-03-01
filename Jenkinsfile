pipeline {
	agent any
	options {
		skipStagesAfterUnstable()
	}
	stages {
		stage('Build') {
			steps {
				echo 'Building ...'
			}
		}
		stage('Test') {
			steps {
				echo 'Testing, 1, 2, 3 ...'
			}
		}
		stage('Deploy') {
			steps {
				echo 'Deploying ...'
			}
		}
	}
}
