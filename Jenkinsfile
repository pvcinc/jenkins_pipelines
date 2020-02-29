pipeline {
	agent { docker { image 'golang' } }
	stages {
		stage('Build') {
			sh 'go version'
		}
	}
}
