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
        always {
            archiveArtifacts artifacts: './build/App/**'
        }
    }
}