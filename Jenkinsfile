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
                // Example: For Java + Maven project
                // sh 'mvn clean package'
                sh 'echo "Build done"'
            }
        }

        stage('Test') {
            steps {
                echo "🧪 Running unit tests..."
                // Example: Java project
                // sh 'mvn test'
                sh 'echo "Tests passed"'
            }
        }

        stage('Deploy') {
            steps {
                echo "🚀 Deploying ${env.APP_NAME} to ${env.ENV}..."
                // Example: deploy using SCP or kubectl
                sh 'echo "Deploy complete"'
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
}
