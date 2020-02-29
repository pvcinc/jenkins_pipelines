pipeline {
	agent any
	stages {
		stage('Fail') {
			steps {
				sh 'echo "Fail!"; exit 1'
			}
		}
	}
	post {
		always {
			echo 'this always executes'
		}
		success {
			echo 'this executes if the run succeeds'
		}
		failure {
			echo 'this executes if the run failed'
		}
		unstable {
			echo 'this executes if the run is unstable'	
		}
		changed {
			echo 'this executes if the pipeline state changed'
			echo 'e.g. the pipeline was failing and now succeeds'
			echo 'e.g. the pipeline was succeeding and now fails'
		}
	}
}
