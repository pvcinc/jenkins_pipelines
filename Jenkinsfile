pipeline {
	agent any
	stages {
		stage('Run Multiple Steps') {
			steps {
				sh 'echo Executing command 1...'
				sh '''
				    echo "Executing command 2..." 
				    echo "Executing command 3..."
				    echo "Executing command N..."
                                    ls -lah
				'''
			}
		}
	}
}
