pipeline{
    agent any
    tools {
        terraform 'Terraform'
    }
    stages{
        stage('Git Checkout'){
            steps{
                git 'https://github.com/EVG-cmd/-test-master'
            }
        }
        stage('Terraform Init'){
            steps{
                sh 'terraform init'
            }
        }
        stage('Terraform Apply'){
            steps{
                sh 'terraform apply --auto-approve'
            }
        }
    
    }
}
