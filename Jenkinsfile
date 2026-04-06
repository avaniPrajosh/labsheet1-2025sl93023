pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/avaniPrajosh/labsheet1-2025sl93023.git'
            }
        }

        stage('Build') {
            steps {
                sh 'echo "Build Stage"'
            }
        }

        stage('Test') {
            steps {
                sh '''
                python3 calculator.py
                '''
            }
        }

        stage('Deploy') {
            steps {
                sh 'echo "Deploy Stage"'
            }
        }
    }
}
