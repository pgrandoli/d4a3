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
				sudo docker build - < /home/backup/php54/Dockerfile
				sudo docker cp /home/backup/d4a/code/index.php 74bea10c3595:/var/www/html
				sudo docker cp /home/backup/d4a/code/db.php 74bea10c3595:/var/www/html
				
			}
		}
			stage('Deploy Container'){
				steps{
					
			}
		}
	}
}
