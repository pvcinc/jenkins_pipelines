node('docker') {
	checkout scm
	stage('Build') {
		docker.image('hello-world')
	}
}
