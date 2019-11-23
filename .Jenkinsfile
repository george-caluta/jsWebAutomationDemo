pipeline {
    agent {
	    	label 'ubuntu18'
		}
				stages {
						stage('Build') {
								steps {
										sh '''
												echo 'Building..'
												apt install npm -y
												npm run start
												npm run test
										'''
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
				}
}
