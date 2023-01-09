pipeline {
	agent any
	
	stages {
	
		stage("build") {
			
			steps {
					echo "Building the application"
			}
		}
		stage("test") {
			
			steps {
					echo "Testing the application"
			}
		}
		stage("deploy") {
			
			steps {
					echo "Deploying the application"
			}
		}
	}
	post {
		always {
		echo "build is completed"
		}
		success {
			echo "This is success block"
		}
		failure {
		 echo "This is failure block"
		}
	}
}
