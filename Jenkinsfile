pipeline{
	agent any

	environment{
		dockerHome = tool 'docker'
		mavenHome = tool 'maven3'
		PATH = "$dockerHome/bin:$mavenHome/bin:$PATH"
	}

	stages{
		stage('Build') {
			steps{
				sh 'mvn --version'
				sh 'docker version'
				
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