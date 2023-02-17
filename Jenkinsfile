pipeline
{
	agent any
	stages
    {
		stage ('Build')
        {
            steps
            {
                sample.cpp -o task5'
                echo 'Build stage Successful'
                build job: 'PES2UG20CS374-1'
            }
        }
		
        stage ('Test')
        {
            steps
            {
                sh './task5'
                echo 'Test successful'
            }
        }
		
        stage('Deploy') 
		{
            steps {
                sh 'echo "Deployment Successful"'
            }
        }
    }
	
post {
        always {
            echo 'Pipeline Successful Completed!'
        }
        failure {
            echo 'Pipeline has failed.'
        }
    }
}
