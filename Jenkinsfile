pipeline {
    agent any

    stages {

        stage('Install Dependencies') {
            steps {
                sh 'cd fullstack-project/backend && npm install'
            }
        }

        stage('Run Application') {
            steps {
                sh 'nohup node fullstack-project/backend/server.js &'
            }
        }

    }
}
