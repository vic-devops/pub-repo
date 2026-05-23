pipeline {
    agent any // Run on any available Jenkins agent

    environment {
        CI = 'true' // Define environment variables
    }

    stages {
        stage('Build') {
            steps {
                echo 'Compiling...'
                sh 'npm install' // Execute shell commands
            }
        }
        stage('Test') {
            steps {
                echo 'Testing...'
                sh 'npm test'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying to production...'
            }
        }
    }

    post { // Actions to take after pipeline finishes
        always {
            echo 'I will always run!'
        }
        success {
            echo 'Pipeline succeeded!'
        }
        failure {
            echo 'Pipeline failed!'
        }
    }
}

