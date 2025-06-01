pipeline {
    agent {
        label 'docker-enabled-agent'
    }

    stages {
        stage('Docker Version') {
            steps {
                sh 'docker --version'
            }
        }
        stage('Pull Node Image') {
            steps {
                sh 'docker pull node:14'
            }
        }
        stage('Run Node Container') {
            steps {
                sh 'docker run --rm node:14 node --version'
            }
        }
    }
}
