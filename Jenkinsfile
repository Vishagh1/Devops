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
            publishHTML(Targets: [
                reportDir: '.',
                reportFiles: 'index.html',
                reportName: 'htmlpage'
                ])
        }
    }
    
}
