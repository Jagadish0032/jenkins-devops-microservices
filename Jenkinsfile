pipeline {
	agent any
	// agent { docker { image 'maven:3.6.3'} }
	// agent { docker { image 'node:13.8'} }
	stages {
		stage('Build'){
			steps {
				// sh 'mvn --version'
				// sh 'node --version'
               echo "Build"
			   echo "PATH - $PATH"
			   echo "BUILD NUMBER -$env.BUILD_NUMBER"
			   echo "BUILD_ID - $env.BUILD_ID"
			   echo "JOB_NAME - $env.JOB_NAME"
			   echo "BUILD_TAG - $env.BUILD_TAG"
			   echo "BUILD_URL - $env.BUILD_URL"		
			   }
		}
		stage('Test'){
			steps{
        echo "Test"
		}
		}
		stage('Integration test'){
			steps{
        echo "Integration Test"
		}
		}
	} 
	post {
		always {
			echo "Iam awesome, I run always"
		}
		success {
			echo "I run when youare successful"
		}
		failure {
			echo "I run when you fail"
		}
	}
	
}
