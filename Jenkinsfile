pipeline{
    agent any
    
    stages{
        stage('TerraformInit'){
            steps{
			echo "Running ${env.BUILD_ID} on ${env.WORKSPACE}"
			sh 'pwd'
			sh 'cd jenkins'
			sh 'cd ${env.WORKSPACE}/jenkins'
			sh 'pwd'
			sh 'terraform init'

                
            }
        }
    }
    
}