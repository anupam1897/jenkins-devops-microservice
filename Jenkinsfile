pipeline{
	agent {
		docker {
			image 'maven:3.6.3'
		}
	}
	stages{
		stage('Build') {
			steps{
				sh 'mvn --version'
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