//script  -old way
//node {
	//echo "Build"
	//echo "Test"
	//echo "Integration Test"
//}

//declarative
pipeline {
	//agent any
	//agent { docker { image 'maven:3.6.3'} }
	stages {
		stage('Build') {
			steps {
				//sh 'mvn --version'
				echo "Build"
				echo "PATH - $PATH"
				echo "BUILD_NUMBER - $env.BUILD_NUMBER"
				echo "BUILD_ID - $env.BUILD_ID"
				echo "JOB_NAME - $env.JOB_NAME"
				echo "BUILD_TAG - $env.BUILD_TAG"
				echo "BUILD_URL - $env.BUILD_URL"
			}
		}
		stage('Test') {
			steps {
				echo "Test"
			}
			
		}
		stage('Integration Test') {
			steps {
				echo "Test"
			}
		}
	} 
	
	post {
			always {
				echo 'Im awesome. I run always'
			}
			success {
				echo 'I run when you are successful'
			}
			failure {
				echo 'I run when you fail'
			}
	}
	
	
}
