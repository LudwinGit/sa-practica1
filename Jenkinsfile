pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'npm install'
            }
        }
        stage('Test') {
            steps {
                sh 'yarn test --watchAll=false'
            }
        }
        stage('Deploy') {
            steps {
                sh 'pm2 start npm --name "app name" -- start'
            }
        }
    }
}