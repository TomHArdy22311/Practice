pipeline {
    agent any 

    tools {
        nodejs 'Simon'
    }

    stages {
        stage('Git') {
            steps {
                git branch: 'main', url: 'https://github.com/TomHArdy22311/Practice.git'
            }
        }

        stage('pm2 installation') {
            steps {
                sh 'npm i pm2 -g'
            }
        }

        stage('pm2 start') {
            steps {
                sh 'npm i'
                sh 'pm2 start index.js --name Rock'
            }
        }
    }
}