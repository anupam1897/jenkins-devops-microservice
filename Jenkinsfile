pipeline{
	agent any
	stages{
		stage('Build') {
			steps{
				echo "Build"
			}
		}
		stage('Test') {
			steps{
				echo "Unit Test"
			}
		}
		stage('Integration Test') {
			steps{
				echo "Integration Test"
			}
		}	
	}
	post{
		always{
			echo "I'm awesome. Run Always"
		}
	}
}