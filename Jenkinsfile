pipeline {
    agent {
        node {
            label 'nodejs'
        }
    }
    stages {
        stage('Checkout') {
            steps {
                git url: 'https://github.com/do400-gunnar/DO400-apps', branch: 'scripted-pipelines'
            }
        }
        stage('Test') {
            steps {
                sh 'simple-webapp/backend/test_api.sh'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying...'
            }
        }
    }
}
