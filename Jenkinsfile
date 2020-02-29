pipeline {
	agent any
	stages {
		stage('RetryStepWithTimeout') {
			steps {
				timeout(time: 3, unit: 'SECONDS') {
					retry(5) {
						sh 'echo "The max time to try this step 5 times is 3 seconds"'
					}
				}
			}
		}
	}
}
