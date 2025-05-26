pipeline{
    agent any

    triggers{
        cron('H/5 * * * *')
        pollSCM('H/2 * * * *')
        githubPush()
    }

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
}
