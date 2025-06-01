pipeline {
    agent any

    environment {
        APP_NAME = "MyApp"
        ENV = "dev"
    }

    stages {
        stage('Clone Repo') {
            steps {
                echo " Cloning repository..."
                checkout scm
            }
        }

        stage('Build') {
            steps {
                echo " Building ${env.APP_NAME} for ${env.ENV}..."
                bat 'echo Build done'
            }
        }

        stage('Test') {
            steps {
                echo " Running unit tests..."
                bat 'echo Tests passed'
            }
        }

        stage('Deploy') {
            steps {
                echo " Deploying ${env.APP_NAME} to ${env.ENV}..."
                bat 'echo Deployed!'
            }
        }
    }

    post {
        success {
            echo " Pipeline finished successfully"
        }
        failure {
            echo " Pipeline failed"
        }
    }
}
