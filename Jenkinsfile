pipeline {
    agent {
        node {
            label 'nodejs'
        }
    }
    stages {
        stage('Checkout') {
            git url: 'https://github.com/do400-gunnar/DO400-apps', branch: 'main'
        }
        stage('Backend Test') {
            sh 'node ./backend/test.js'
        }
        stage('Deploy') {
            echo 'Deploying...'
        }
    }
}
