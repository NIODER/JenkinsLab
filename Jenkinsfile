pipeline {
    agent {
        docker {
            image
        }
    }
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