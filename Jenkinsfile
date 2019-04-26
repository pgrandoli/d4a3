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
				sudo docker run 81b89a3d84b0
				cp /home/backup/d4a/code/* /var/www/html/
				sudo docker build --tag=php .
				
			}
		}
			stage('Deploy Container'){
				steps{
					
			}
		}
	}
}
