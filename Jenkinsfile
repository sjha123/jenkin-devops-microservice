//node {
//	stage('Build') {
//		echo "Build"
//	}
//	stage('Test') {
//		echo "Test"
//	}
//	stage('IntegrationTest') {
//		echo "IntegrationTest"
//	}
//}
pipeline {
	agent any 

	stages{
			stage('Build'){
				steps {
				echo "Build"
				echo "Path - $PATH"
				echo "Build No- $env.BUILD_NUMBER"
				echo "Build ID- $env.BUILD_ID"
				echo "job Name- $env.JOB_NAME"
			 }
		}
		
		stage('Test'){
				steps {
				echo "Test"
			 }
		}
	}

	post{
        always 
		{
			echo "I will run always"
		}
		success
		{
			echo "I will run when success"
		}
		failure
		{
		   echo "I will run when PIPLINE FAILED"
		}

	}


}


