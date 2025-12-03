pipeline {
    agent any

    environment {
        IMAGE_NAME = "swiggy-clone"
    }

    stages {

        stage('Checkout') {
            steps {
                git branch: 'main',
                    url: 'https://github.com/Ankitpandey321/swiggy-clone.git'
            }
        }

        stage('Build Docker Image') {
            steps {
                sh 'docker build -t $DOCKERHUB_USER/$IMAGE_NAME:latest .'
            }
        }
    }

    post {
        always {
            echo "Pipeline finished"
        }
    }
}
