pipeline {
    agent {
        docker {
	    	image 'jenkinsci/jnlp-slave'
	    	label 'node'
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
