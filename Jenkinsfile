pipeline {
    agent any
    stages {
        stage('Clone code') {
            steps {
                git 'https://github.com/nhathoang1505/jenkins-demo.git'
            }
        }
        stage('Install dependencies') {
            steps {
                sh 'pip install pytest'
            }
        }
        stage('Run tests') {
            steps {
                sh 'pytest test_calculator.py'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploy thành công 🚀'
            }
        }
    }
}
