pipeline{
	environment{
		registry = "pgrandoli/d4a3"
		registryCredential = "dockerhub"
	}
	agent any
	stages{
			stage('Starting'){
				steps{
				sh 'echo starting...'
			}
		}
			stage('Checking Docker'){
				steps{
				sh 'sudo docker ps'
			}
		}
			stage('Build image'){
				steps{
					script{
						dockerImage=docker.build registry + ":$BUILD_NUMBER"
					}	
			}
		}
			stage('Deploy Container'){
				steps{
				sh 'echo'	
			}
		}
	}
}
