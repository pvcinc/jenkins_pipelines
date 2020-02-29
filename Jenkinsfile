pipeline {
	agent any
	stages {
		stage('RetryStepWithTimeout') {
			steps {
				timeout(time: 3, unit: 'SECONDS') {
					retry(5) {
						sh 'echo "The max time to try this step 5 times is 3 seconds"'
						sh 'echo "A Failure occured!"; exit 1'
					}
					sh 'sleep 4'
				}
			}
		}
	}
}
