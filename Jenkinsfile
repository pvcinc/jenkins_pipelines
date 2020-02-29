pipeline {
	agent any
	stages {
		stage('StepWithRetries') {
			steps {
				retry(3) {
					sh 'echo "If this step failed Jenkins would try again 3 times"'
					sh 'echo "Fail!"; exit 1'
				}
			}
		}
	}
}
