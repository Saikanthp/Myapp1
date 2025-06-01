pipeline {
    agent {
        docker {
            image 'maven:3.8.4-jdk-11'  // Use Maven image with JDK 11
            label 'docker'              // Optional: node label to run this on
            args '-v /root/.m2:/root/.m2' // Mount volume to cache Maven dependencies
        }
    }
    stages {
        stage('Build') {
            steps {
                echo 'Building inside Docker container...'
                sh 'mvn -version'         // Run Maven command inside container
            }
        }
        stage('Test') {
            steps {
                echo 'Testing inside Docker container...'
                sh 'echo Running tests...'
            }
        }
    }
}
