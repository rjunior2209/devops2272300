pipeline{
    agent any
    stages{
        stage('Build TADS'){
            steps{
                bat'''
                java --version
                docker --version
                docker compose version
                docker info
                '''
            }
        }
    }
}