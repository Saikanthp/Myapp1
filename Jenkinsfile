pipeline {
    agent any

    environment {
        MY_ENV_VAR = "This is a custom env variable"
    }

    stages {
        stage('Show Env Variables') {
            steps {
                echo "🏷️ Job Name: ${env.JOB_NAME}"
                echo "📁 Workspace: ${env.WORKSPACE}"
                echo "🔢 Build Number: ${env.BUILD_NUMBER}"
                echo "🧪 Custom Var: ${env.MY_ENV_VAR}"
            }
        }

        stage('Use GitHub Token') {
            steps {
                withCredentials([string(credentialsId: 'GITHUB-TOKEN', variable: 'GITHUB-TOKEN')]) {
                    echo "🔒 GitHub Token Length: ${GITHUB-TOKEN.length()}"
                }
            }
        }
    }
}
