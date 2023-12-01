pipeline{

    agent any
       tools {nodejs 'slameubom'}

    stages {
        stage('Start NodeGoat') {
            steps {
                sh '''
                        npm install
                '''
            }
        }
        stage('Test NPM') {
            steps {
                sh '''
                    npm test
                '''
            }
        }
        stage('Construindo Docker') {
            steps {
                sh '''
                    docker build .
                '''
            }
        }
        stage('Compose Docker') {
            steps {
                sh '''
                    docker compose up
                '''
            }
        }
    }
}