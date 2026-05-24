pipeline {
    agent any // Run on any available Jenkins agent

    // environment {
    //     CI = 'true' // Define environment variables
    // }

    stages {
        // stage('Build') {
        //     steps {
        //         echo 'Compiling...'
        //         sh 'sudo install nginx -y' // Execute shell commands
        //     }
        // }
        stage('Test') {
            steps {
                echo 'Testing...'
                sh 'ls -a'
            }
        }
        stage('Deploy') {
            steps {
                echo 'i want my deployment'
                sh 'cat /etc/passwd'
            }
        }
    
    }
}

