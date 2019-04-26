pipeline{
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
				sh 'sudo docker build --tag=phpp .'	
			}
		}
			stage('Deploy Container'){
				steps{
				sh 'echo'	
			}
		}
	}
}
