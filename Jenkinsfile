pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
		stage('Read Me File '){
		    when {
			  branch "Test-2"
			}
			steps {
			  sh'''
			  cat readme.txt
			  '''
			}
		}
    }
}
