pipeline{
    agent any
    
    stages{
        stage('TerraformInit'){
            steps{
			sh 'terraform init ${WORKSPACE}/jenkins'

                
            }
        }
    }
    
}