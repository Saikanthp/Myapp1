pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Building the application...'
                // Add your build commands here, e.g. mvn clean package
            }
        }
        stage('Test') {
            steps {
                echo 'Running tests...'
                // Add your test commands here, e.g. mvn test
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying application...'
                // Add your deploy commands here, e.g. copy files, docker build/push
            }
        }
    }
}
