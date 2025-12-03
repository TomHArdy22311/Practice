pipeline {
    agent any 

    tools {
        nodejs 'Simon'
    }

    stages {
        stage('pm2 installation') {
            steps{
                sh 'npm i pm2 -g'
            }
        }

        stage('pm2 start') {
            steps {
                sh 'pm2 start index.js --name Rock'
            }
        }
    }
}