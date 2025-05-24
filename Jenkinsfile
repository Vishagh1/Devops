pipeline {
    agent any

    stages {
        stage('Pull HTML') {
            steps {
                echo 'Fetching HTML page'
            }
        }
    }

    post {
        success {
            publishHTML(target: [
                reportDir: '.',
                reportFiles: 'index.html',
                reportName: 'My HTML Page'
            ])
        }
    }
}
