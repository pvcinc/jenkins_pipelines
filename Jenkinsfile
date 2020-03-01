pipeline {
    agent any
    stages {
        stage('SucceedingStage') {
            steps {
                echo "I ran successfully"
            }
        }
    }
    post {
        success {
            slackSend channel: '#ci_cd_build',
                      color: 'good',
                      message: "The pipeline $currentBuild.fullDisplayName was successful"
        }
    }
}
