pipeline {
    agent any

    stages {

        stage('Clone Repository') {
            steps {
                git 'https://github.com/giriprasanna7/fullstack-jenkins.git'
            }
        }

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
