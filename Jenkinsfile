pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh '''
                    docker compose build
                    docker compose up
                '''
            }
        }
    }
    post {
        archiveArtifacts artifacts: './build/App/**'
    }
}