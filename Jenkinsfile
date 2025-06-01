pipeline {
    agent any

    environment {
        APP_NAME = "MyApp"
        ENV = "dev"
    }

    stages {
        stage('Clone Repo') {
            steps {
                echo "📥 Cloning repository..."
                checkout scm
            }
        }

        stage('Build') {
            steps {
                echo "🔧 Building ${env.APP_NAME} for ${env.ENV}..."
                sh 'echo Build done'
            }
        }

        stage('Test') {
            steps {
                echo "🧪 Running unit tests..."
                sh 'echo Tests passed'
            }
        }

        stage('Deploy') {
            steps {
                echo "🚀 Deploying ${env.APP_NAME} to ${env.ENV}..."
                sh 'echo Deployed!'
            }
        }
    }

    post {
        success {
            echo "✅ Pipeline finished successfully"
        }
        failure {
            echo "❌ Pipeline failed"
        }
    }
}
