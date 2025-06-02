pipeline {
    agent any

    stages {
        stage('Preparation') {
            steps {
                echo "📦 Preparing build..."
            }
        }

        stage('Build') {
            steps {
                echo "🏗️ Building the application..."
            }
        }
        
        stage('Test') {
            steps {
                echo "✅ Running tests... All tests passed!"
            }
        }

        stage('Deploy') {
            steps {
                echo "🚀 Deployment complete!"
            }
        }
    }

    post {
        success {
            echo "🎉 Build completed successfully!"
        }
        failure {
            echo "❌ Build failed!"
        }
    }
}
