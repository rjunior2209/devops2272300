pipeline{
    agent any
    stages{
        stage('Build TADS'){
            steps{
                sh '''
                java --version
                docker --version
                doker-compose
                docker info
                docker compose version
                '''
            }
        }
    }
}