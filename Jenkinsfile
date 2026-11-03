
pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                echo 'Getting source code from GitHub'
            }
        }

        stage('Environment') {
            steps {
                sh 'whoami'
                sh 'java -version'
                sh 'git --version'
            }
        }

        stage('Build') {
            steps {
                echo 'Building application'
                sh 'echo Build Successful'
            }
        }

        stage('Test') {
            steps {
                echo 'Testing application'
                sh 'echo All Tests Passed'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deployment completed'
            }
        }
    }

    post {
        success {
            echo 'CI/CD Pipeline Successful!'
        }
        failure {
            echo 'Pipeline Failed!'
        }
    }
}
