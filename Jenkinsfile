pipeline {
    agent any

    stages {

        stage('Install Dependencies') {
            steps {
                sh 'cd backend && npm install'
            }
        }

        stage('Run Application') {
            steps {
                sh 'nohup node backend/server.js &'
            }
        }

    }
}
