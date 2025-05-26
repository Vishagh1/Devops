pipeline{
    agent any


    stages{
        stage('Build'){
            steps{
                echo "Building.."
            }
        }

        stage('Deploy'){
            steps{
                echo "Deploying"
            }
        }
    }

    post{
        success{
            publishHTML(target: [
                reportDir: '.',
                reportFiles: 'index.html',
                reportName: 'htmlpage'
                ])
        }
    }
    
}
