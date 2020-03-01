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
				echo 'Unit Testing 1, 2, 3...' 
			}
		}
		stage('Deploy to Staging') {
			steps { 
				echo 'Deploying to Staging Environment ...'
				echo 'Smoke Testing 1, 2, 3...'
			 }
		}		
		stage('Deploy to Production') {
			steps { 
				echo 'Deploying to Production Environment ...' 
			}		
		}
	}
}
