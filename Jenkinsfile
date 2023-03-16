pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', credentialsId: 'ssh key', url: 'git@github.com:aafaq-rana-01/jenkins-pipeline-private.git'
            }
        }
        stage('Build') {
            steps {
                bat 'python test.py'
            }
        }
    }
}
