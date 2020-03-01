pipeline {
    agent any
    stages {
        stage('FailingStage') {
            steps {
                echo "A Failure Occured!"
                exit 1
            }
        }
    }
    post {
        failure {
            mail to: '$USERNAME@DOMAIN',
            subject: "Failed Pipeline: $currentBuild.fullDisplayName",
            body: "Please check $env.BUILD_URL"
        }
    }
}
