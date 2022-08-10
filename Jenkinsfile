pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo "Building.. ${BUILD_ID}"
                wrap([$class: 'BuildUser']) {
                    sh 'echo "${BUILD_USER}"'
                }
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