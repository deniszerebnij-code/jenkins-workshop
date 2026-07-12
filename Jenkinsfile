pipeline {
    agent {
        docker { image 'hashicorp/terraform:latest' }
    }
    stages {
        stage('Checkout Code') {
            steps { checkout scm }
        }
        stage('Terraform Version') {
            steps { sh 'terraform version' }
        }
        stage('Terraform Init') {
            steps { sh 'terraform init' }
        }
    }
}