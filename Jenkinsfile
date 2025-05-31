pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh '''echo "compiling java project..."
java App.java
'''
      }
    }

    stage('Test') {
      steps {
        echo 'Running tests...'
        sh '''echo "Running test"
java App
'''
      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploying application...'
        sh '''echo"deploying the application"
'''
      }
    }

  }
}