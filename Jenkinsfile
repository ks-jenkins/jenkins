pipeline {
    agent any

    stages {
        stage('Terraform Install'){
            steps {
                sh 'pwd'
                sh 'whoami'
                sh 'terraform --version'
            }
        }
        stage('Build') {
            steps {
                wrap([$class: 'BuildUser']) {
                    sh '''
                    echo "${BUILD_USER}"
                    echo "My Name"
                    '''
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