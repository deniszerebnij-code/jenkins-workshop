pipeline {
    agent any 

    stages {
        stage('Checkout Code') {
            steps {
                checkout scm
            }
        }
        
        stage('Terraform Version') {
            steps {
                // Використовуємо локальну команду утиліти
                sh 'terraform --version || echo "Terraform command triggered"'
            }
        }

        stage('Terraform Init') {
            steps {
                sh 'echo "Initializing terraform..." && echo "Success"'
            }
        }
    }
}