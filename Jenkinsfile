pipeline {

    agent any

    stages {

        stage('Checkout Code') {
            steps {
                git branch: 'main',
                url: 'https://github.com/meghanau09/sample-node-app.git'
            }
        }

        stage('Build Docker Image') {
            steps {
                bat 'docker build -t sample-node-app .'
            }
        }

        stage('Deploy Container') {
            steps {
        bat '''
        docker stop sample-node-container
        IF %ERRORLEVEL% NEQ 0 echo Container not running

        docker rm sample-node-container
        IF %ERRORLEVEL% NEQ 0 echo Container does not exist

        docker run -d -p 3000:3000 --name sample-node-container sample-node-app

        docker ps
        '''
            }
        }
    }
}