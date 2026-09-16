node('nodejs') {
    stage('Say Hello') {
        echo 'Hello'
    }
    stage('List it') {
        sh 'tree .'
    }
    stage('Backend Test') {
        sh 'node ./backend/test.js'
    }
    stage('Deploy') {
        echo 'Deploying...'
    }
}
