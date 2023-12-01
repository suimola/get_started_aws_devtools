pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/suimola/get_started_aws_devtools.git'
            }
        }

        stage('Install dependencies') {
            steps {
                sh 'npm install'
            }
        }

        stage('Start server') {
            steps {
                sh 'node app.js'
            }
        }
    }
}
