CODE_CHANGE = getGitChanges()
BRANCH_NAME = 'dev'


pipeline {
	agent any
	
	stages {
	
		stage("build") {

			expression {
				BRANCH_NAME == 'dev' || CODE_CHANGE == true
			}
			
			steps {
					echo "Building the application"
			}
		}
		stage("test") {
			expression {
				BRANCH_NAME == 'dev'
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
