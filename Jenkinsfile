pipeline{
    agent any
    
    stages{
        stage('TerraformInit'){
            steps{
			echo "Running ${env.BUILD_ID} on ${env.WORKSPACE}"
			sh 'pwd'
			sh 'cd $workspace/jenkins; pwd'
			sh 'pwd'
			sh 'terraform init'

                
            }
        }
    }
    
}