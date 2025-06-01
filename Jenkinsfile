pipeline {
    agent any

    stages {
        stage('Docker Version') {
            steps {
                echo 'Checking Docker version...'
                bat 'docker --version'
            }
        }

        stage('Pull Node Image') {
            steps {
                echo 'Pulling node:20 image...'
                bat 'docker pull node:20'
            }
        }

        stage('Run Node Container') {
            steps {
                echo 'Running node container and checking version...'
                bat 'docker run --rm node:20 node --version'
            }
        }
    }
}
