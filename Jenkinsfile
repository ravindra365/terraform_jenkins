pipeline{
    agent any
    
    stages{
		stage('Credential Manager AWS') {
            environment{
                My_User_Credentials = credentials('secret_id')
            }
            steps {
                sh "aws configure set aws_access_key_id $My_User_Credentials_USR"
                sh "aws configure set aws_secret_access_key $My_User_Credentials_PSW"
                sh "aws configure list"
            }
        }
		
        stage('TerraformInit'){
            steps{
			echo "Terraform init"
			sh "cd ${env.WORKSPACE}/jenkins; terraform init"  
            }
        }
		
		stage('Terraform fmt'){
			steps{
			echo "Terraform reformat configuration"
			sh "cd ${env.WORKSPACE}/jenkins; terraform fmt"  
			}
		}
		
		stage('Terraform apply'){
			steps{
			echo "Terraform reformat configuration"
			sh "cd ${env.WORKSPACE}/jenkins; terraform apply"  
			}
		}
    }
    
}