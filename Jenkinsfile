pipeline {
    agent any

    stages {
        stage('NpmInstall') {
            steps {
                sh 'npm install'
            }
        }
        stage('Build') {
            steps {
                sh 'npm run build:prod'
            }
        }
        stage('Zip') {
            steps {
                sh 'npm run zip'
            }
        }
    }
}