pipeline {
    agent {
        docker-cloud {
            image 'node:latest'
            label 'my-defined-label'
            args  '-v /tmp:/tmp'
        }
		}
				stages {
						stage('Build') {
								steps {
										sh '''
												echo 'Building..'
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
