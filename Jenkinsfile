pipeline{
    agent any
    
    stages{
        stage('TerraformInit'){
            steps{
			sh 'pwd'
			sh 'cd ${WORKSPACE}/jenkins'
			sh 'terraform init'

                
            }
        }
    }
    
}