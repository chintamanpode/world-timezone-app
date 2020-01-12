pipeline{
		agent any
		stages{
			stage('Build Application'){
				steps{
					sh 'mvn clean install'
				}
			}

			stage('Munit Testing Application'){
				steps{
					sh 'mvn test'
				}
			}

			stage('Deploy Application To Mulesoft Cloudhub'){
				steps{
					sh 'mvn package deploy -DmuleDeploy'
				}
			}					
		}				
}

	