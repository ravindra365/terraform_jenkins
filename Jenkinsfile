pipeline{
    agent any
    
    stages{
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