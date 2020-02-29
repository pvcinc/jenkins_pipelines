pipeline {
	agent { docker { image 'php' } }
	stages {
		stage('Build') {
			steps {
				sh 'php --version'
			}
		}
	}
}
