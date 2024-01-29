pipeline {
    agent any
    
    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/Ahtishamsaleem/jenkin-sonarcube-docker.git'
            }
        }
        
        stage('Build') {
            steps {
                // Your build commands here
            }
        }
        
        stage('Deploy') {
            steps {
                sh 'sudo cp -r * /var/www/html/'
                sh 'sudo service httpd restart'
            }
        }
    }
    
    post {
        success {
            echo 'Build and deployment successful!'
        }
        failure {
            echo 'Build or deployment failed!'
        }
    }
}
