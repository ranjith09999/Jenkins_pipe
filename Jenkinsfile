CODE_CHANGE = getGitChanges()
BRANCH_NAME = 'dev'


pipeline {
	agent any
	
	stages {
	
		stage("build") {
			when {
			expression {
				BRANCH_NAME == 'dev' || CODE_CHANGE == true
			}
			}
			steps {
					echo "Building the application"
			}
		}
		stage("test") {
			when {
			expression {
				BRANCH_NAME == 'dev'
			}
			}
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
}
