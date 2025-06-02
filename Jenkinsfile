pipeline {
    agent any
    environment {
        GITHUB_TOKEN = credentials('GITHUB_TOKEN') // matches the ID you gave
    }
    stages {
        stage('Show Token Length') {
            steps {
                echo "GitHub Token Length: ${GITHUB_TOKEN.length()}"
            }
        }
    }
}
