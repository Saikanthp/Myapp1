pipeline {
  agent any
  parameters {
    choice(name: 'ENV', choices: ['dev', 'qa', 'prod'], description: 'Environment to deploy')
  }
  stages {
    stage('Show Parameter') {
      steps {
        echo "Selected Environment: ${params.ENV}"
      }
    }
    // other stages like build, test, deploy...
  }
}
