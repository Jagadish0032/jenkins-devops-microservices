pipeline {
	agent any
	stages {
		stage('Build'){
			steps {
               echo "Build"
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
	} post {
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
