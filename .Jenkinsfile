agent {
    docker-cloud {
        image 'node:8.16.2-alpine3.9'
        label 'my-defined-label'
        args  '-v /tmp:/tmp'
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
