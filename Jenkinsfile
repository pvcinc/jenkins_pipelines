pipeline {
	agent any
	stages {
		stage('FailingStage') {
			step {
				echo "A Failure Occured!"
				exit 1
			}
		}
	}
	post {
		failure {
			mail to: jacobitegboje@gmail.com.
			subject: "Failed Pipeline: ${currentBuild.fullDisplayName}",
			body: "Please check ${env.BUILD_URL}"
		}
	}
}
