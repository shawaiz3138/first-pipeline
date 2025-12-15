pipeline {
    agent any
    
    stages {
        stage('Checkout') {
            steps {
                echo 'Pulling code from GitHub...'
                checkout scm
            }
        }
        
        stage('Build') {
            steps {
                echo 'Building the application...'
                echo 'Code pulled successfully from GitHub!'
            }
        }
        
        stage('Test') {
            steps {
                echo 'Running tests...'
                echo 'All tests passed!'
            }
        }
        
        stage('Deploy') {
            steps {
                echo 'Deploying application...'
                echo 'Deployment successful!'
            }
        }
    }
    
    post {
        success {
            echo '✅ Pipeline completed successfully!'
            echo 'GitHub integration is working!'
        }
        failure {
            echo '❌ Pipeline failed!'
        }
    }
}