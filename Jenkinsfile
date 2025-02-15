pipeline {
    agent {
        docker { image 'node:16-alpine' }
    }
    stages {
        stage('Checkout Code') {
            steps {
                git branch: 'main', url: 'https://github.com/YOUR_GITHUB_USERNAME/jenkins-pipeline-demo.git'
            }
        }
        stage('Test Code') {
            steps {
                sh 'node --version'
            }
        }
        stage('Build & Deploy') {
            steps {
                sh 'echo Deploying App...'
            }
        }
    }
}
