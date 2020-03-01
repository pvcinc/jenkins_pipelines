pipeline {
	agent {
		docker { image 'node:7-alpine' }
	}

	stages {
		stage('DockerWorkspace') {
			steps {
				sh 'node --version'
				sh 'pwd'
				sh 'whoami'
			}
		}
	}
}
