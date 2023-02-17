pipeline {
  agent any
	 stages {
		 stage('Build') {
		 steps {
			 sh 'g++ -o PES2UG20CS374-1 ./sample.cpp'
			 echo 'Build phase successful'
		 }
	 	}
		 stage('Test') {
			 steps {
			 sh './PES2UG20CS374-1'
			 echo 'Test successful'
			 }
		 }
		 stage('Deploy') {
			 steps {
			 eco 'Deployment successful'
			 }
		 }
	}
	
	post {
		always {
		    echo 'Pipeline Successfully Completed!'
		}
		
		failure {
		    echo 'Pipeline failed!!'
		}
	    
	}
}
