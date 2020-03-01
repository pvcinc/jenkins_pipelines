pipeline {
	agent any
	options {
		skipStagesAfterUnstable()
	}
	stages {
		stage('Build') {
			echo 'Building ...'
		}
		stage('Test') {
			echo 'Unit Testing 1, 2, 3...'
		}
		stage('Deploy to Staging') {
			echo 'Deploying to Staging Environment ...'
			echo 'Smoke Testing 1, 2, 3...'
		}		
		stage('Deploy to Production') {
			echo 'Deploying to Production Environment ...'
			
		}
	}
}
