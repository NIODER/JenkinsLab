pipeline {
    agent {
        docker {
            image
        }
    }
    stages {
        stage('Build') {
            steps {
                sh "docker compose build"
            }
        }
    }
}