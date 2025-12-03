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

        stage('pm2 start') {
            steps {
                sh 'npm install'
                sh 'npm start index.js'
            }
        }
    }
}