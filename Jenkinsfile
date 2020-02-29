pipeline {
	agent any
	stages {
		stage('StepWithTimeout') {
			steps {
				timeout(time: 3, unit: 'SECONDS') {
					sh 'The max time for this command to run is 3 seconds'
				}
			}
		}
	}
}
