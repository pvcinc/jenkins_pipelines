pipeline {
	agent any
	stages {
		
		stage('Build') {
			steps {
				echo "I'm Building ..."
			}
		}
		stage('Test') {
			steps {
				echo "I'm unit testing ..."
			}
		}
		stage('Deploy to Staging') {
			steps {
				echo "I'm deploying to staging ..."
			}
		}
		stage('Human Approval') {
			steps {
				echo "I'm waiting for approval to proceed"
				timeout(time: 60, unit: 'SECONDS') {
					input "Does the staging environment look right?"
				}
			}
		}
		stage('Deploy to Production') {
			steps {
				echo "I'm deploy to production ..."
			}
		}
	}
}
