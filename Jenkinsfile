pipeline {
    agent any // Run on any available Jenkins agent

    // environment {
    //     CI = 'true' // Define environment variables
    // }

    stages {

        stage('update') {
            steps {
                echo 'updating'
                sh 'sudo apt update' // Execute shell commands
            }
        }
        stage('install') {
            steps {
                echo 'installation of nginx'
                sh 'sudo apt install nginx -y' // Execute shell commands
            }
        }
        stage('Test') {
            steps {
                echo 'list'
                sh 'ls -a /var/lib/jenkins'
            }
        }
        stage('Deploy') {
            steps {
                echo 'show system users'
                sh 'cat /etc/passwd'
            }
        }
    
    }
}

