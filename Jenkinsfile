pipeline {
    agent any
    stages {
        stage('Lint HTML & Dockerfile'){
            steps {
                sh 'tidy -q -e blue-green/blue/*.html'
                sh 'tidy -q -e blue-green/green/*.html'
                sh 'hadolint blue-green/blue/Dockerfile'
                sh 'hadolint blue-green/green/Dockerfile'
            }
        },
        stage('Build and Publish Docker Image'){
                    steps {
                        sh 'docker build -t herreraluis/blueimage -f blue-green/blue/Dockerfile blue-green/blue'
                        sh 'docker build -t herreraluis/greenimage -f blue-green/green/Dockerfile' blue-green/green'
                        sh 'docker push herreraluis/blueimage'
                        sh 'docker push herreraluis/greenimage'
                        sh 'docker rmi -f herreraluis/greenimage'
                        sh 'docker rmi -f herreraluis/blueimage'
                    }
                }
    }
}
