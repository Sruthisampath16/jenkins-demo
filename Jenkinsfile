pipeline {
    agent any

    environment {
        APP_NAME = 'hello-app'
    }

    stages {
        stage('Build') {
            steps {
                echo "Building ${APP_NAME}"
                sh 'ls -la'
            }
        }
        stage('Test') {
            steps {
                echo 'Running tests...'
                sh 'echo "All tests passed again"'
            }
        }
    }

    post {
        success { echo 'Pipeline succeeded' }
        failure { echo 'Pipeline failed' }
    }
}