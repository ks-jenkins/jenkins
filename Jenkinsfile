pipeline {
    agent any

    stages {
        stage('Terraform Install'){
            steps {
                sh 'pwd'
                sh 'whoami'
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
        stage('Ansible') {
            steps {
                sh 'ansible --version'
            }
        }
        stage('Terraform') {
            steps {
                echo 'Testing..'
                sh 'terraform --version'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}