pipeline {
    agent any

    environment {
        IMAGE_NAME = "swiggy-clone"
        DOCKERHUB_USER = "your-dockerhub-username"
        DOCKERHUB_PASS = "your-dockerhub-password"   // Hard-coded (not secure)
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

        stage('Login and Push') {
            steps {
                sh '''
                    echo $DOCKERHUB_PASS | docker login -u $DOCKERHUB_USER --password-stdin
                    docker push $DOCKERHUB_USER/$IMAGE_NAME:latest
                '''
            }
        }
    }

    post {
        always {
            echo "Pipeline finished"
        }
    }
}
