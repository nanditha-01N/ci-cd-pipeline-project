pipeline {
    agent any
    environment {
        DOCKER_IMAGE = "yourdockerhubusername/ci-cd-demo"
    }
    stages {
        stage('Clone') {
            steps {
                git 'https://github.com/yourusername/ci-cd-pipeline-project.git'
            }
        }
        stage('Build Image') {
            steps {
                sh 'docker build -t $DOCKER_IMAGE .'
            }
        }
        stage('Push Image') {
            steps {
                sh 'docker push $DOCKER_IMAGE'
            }
        }
        stage('Deploy to K8s') {
            steps {
                sh 'kubectl apply -f k8s/'
            }
        }
    }
}
