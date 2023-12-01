pipeline{

    agent any

    stages {
        stage('Install NPM') {
            steps {
                bat '''
                        npm install
                '''
            }
        }
        stage('Test NPM') {
            steps {
                bat '''
                    npm test
                '''
            }
        }
        stage('Construindo Docker') {
            steps {
                bat '''
                    docker build .
                '''
            }
        }
        stage('Compose Docker') {
            steps {
                bat '''
                    docker compose up
                '''
            }
        }
    }
}