pipeline {
    agent any
    environment {
        GITHUB-TOKEN = credentials('GITHUB-TOKEN') // matches the ID you gave
    }
    stages {
        stage('Show Token Length') {
            steps {
                echo "GitHub Token Length: ${GITHUB-TOKEN.length()}"
            }
        }
    }
}
