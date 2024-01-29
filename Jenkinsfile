pipeline {
    agent any
    
    stages {
        stage('Checkout') {
            steps {
                git https://github.com/Ahtishamsaleem/jenkin-sonarcube-docker.git
            }
        }
        
        stage('Build') {
            steps {
                // Your build commands here
            }
        }
        
        stage('Deploy') {
            steps {
                // Your deployment commands here
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
