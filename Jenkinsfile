pipeline {
    agent any

    environment {
        APP_NAME='testapp'
        URL_DOCKERHUB='url'
        USER_NAME='twixie089'
        GIT_URL=''
    }

    stages {
        stage('Stage 1') {
            steps {
                echo 'Hello world!'
            }
        }
        stage('Test') {
            steps {
                echo 'Stage = Test!'
            }
            post {
                always {
                    echo 'Test = OK!'
                }
            }
        }
    }
}
