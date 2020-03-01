pipeline {
    agent {
        label '!windows'
    }
    environment {
        VARIABLE_1 = 'value 1'
        VARIABLE_2 = 'value 2'
        VARIABLE_3 = 'value 3'
        VARIABLE_N = 'value N'
    }
    stages {
        stage('Build') {
            steps {
                echo "The value of Variable 1 is ${VARIABLE_1}"
                echo "The value of Variable 2 is ${VARIABLE_2}"
                echo 'The value of Variable 3 is ${VARIABLE_3}'
                echo "The value of Variable 3 is ${VARIABLE_3}"
                echo "The value of Variable N is $VARIABLE_N"
                sh 'printenv'
            }
        }
    }   
}

