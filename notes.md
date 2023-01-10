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