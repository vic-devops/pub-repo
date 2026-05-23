pipeline {
    agent any // Run on any available Jenkins agent

    // environment {
    //     CI = 'true' // Define environment variables
    // }

    stages {
        stage('Build') {
            steps {
                echo 'Compiling...'
                sh 'sudo install nginx -y' // Execute shell commands
            }
        }
        stage('Test') {
            steps {
                echo 'Testing...'
                sh 'ls'
            }
        }
        stage('Deploy') {
            steps {
                echo 'cat /etc/passwd'
            }
        }
    
    }
}

