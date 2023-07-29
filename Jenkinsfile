pipeline{
    agent any
    
    stages{
        stage('TerraformInit'){
            steps{
			sh 'cd ${WORKSPACE}jenkins/'
			sh 'terraform init'

                
            }
        }
    }
    
}