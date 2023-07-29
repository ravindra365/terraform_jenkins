pipeline{
    agent any
    
    stages{
        stage('TerraformInit'){
            steps{
			echo "Running ${env.BUILD_ID} on ${env.WORKSPACE}"
			sh "cd ${env.WORKSPACE}/jenkins; pwd"
			sh 'pwd'
			sh 'terraform init'

                
            }
        }
    }
    
}