pipeline{
    agent any
    
    stages{
        stage('TerraformInit'){
            steps{
			echo "Terraform init"
			sh "cd ${env.WORKSPACE}/jenkins; terraform init"  
            }
        }
		stage('Terraform Plan'){
			steps{
			echo "Terraform init"
			sh "cd ${env.WORKSPACE}/jenkins; terraform plan"  
			}
		}
    }
    
}