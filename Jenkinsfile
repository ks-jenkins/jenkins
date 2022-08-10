pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo "Building.. ${BUILD_USER}"
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}