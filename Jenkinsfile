pipeline {
    agent any

    stages {
        stage('Update Package Index') {
            steps {
                // Refresh local package lists to get the latest versions
                sh 'sudo apt update'
            }
        }

        stage('Install Nginx') {
            steps {
                // Install Nginx without manual confirmation prompts (-y)
                sh 'sudo apt install -y nginx'
            }
        }

        stage('Verify Installation') {
            steps {
                // Check if Nginx is active and running
                sh 'systemctl status nginx'
                // Confirm Nginx version
                sh 'nginx -v'
            }
        }
    }

    post {
        success {
            echo 'Nginx has been successfully installed and started on Ubuntu!'
        }
        failure {
            echo 'Nginx installation failed. Check the logs for details.'
        }
    }
}

