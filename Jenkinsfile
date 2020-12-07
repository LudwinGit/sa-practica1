pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'yarn install'
            }
        }
        stage('Test') {
            steps {
                sh 'yarn test --watchAll=false'
            }
        }
        stage('Deploy') {
            steps {
                sh 'yarn start'
            }
        }
    }
}
