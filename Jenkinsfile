pipeline {
    agent any

    stages {
        stage('Docker Version') {
            steps {
                echo 'Checking Docker version...'
                sh 'docker --version'
            }
        }

        stage('Pull Node Image') {
            steps {
                echo 'Pulling node:20 image...'
                sh 'docker pull node:20'
            }
        }

        stage('Run Node Container') {
            steps {
                echo 'Running node container and checking version...'
                sh 'docker run --rm node:20 node --version'
            }
        }
    }
}
