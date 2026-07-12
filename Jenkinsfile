pipeline {
    agent {
        docker { image 'hashicorp/terraform:latest' }
    }
    stages {
        stage('Checkout Code') {
            steps { checkout scm }
        }
        stage('Terraform Version') {
            steps { sh 'terraform version' } # Task 7
        }
        stage('Terraform Init') {
            steps { sh 'terraform init' } # Task 7
        }
    }
}