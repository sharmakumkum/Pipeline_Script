pipeline{
	agent any
	stages{
		stage('Git-Checkout'){
			steps{
					echo "Checking out from GIT repo!!!";
				}
		}
		stage('Build'){
			steps{
					echo "Building the source code!!!";
				}
		}
		stage('Unit-Test'){
			steps{
					echo "Running Unit-Test!!!";
				}
		}
		stage('Deploy'){
			steps{
					echo "Depolyed on test server for testing!!!";
				}
		}
	}
	
	post{
		always{
			echo 'This will always run'
		}
		success{
			echo 'This will run only if successful'
		}
		failure{
			echo 'This will run only if failed'
		}
		unstable{
			echo 'This will run if the run was marked as unstable'
		}
		changed{
			echo 'This will run only if the state of pipeline has changed'
			echo 'For example, if the pipeline was previously failing but is now successful'
		}
	}	
}