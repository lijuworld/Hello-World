pipeline {
    agent any

    stages {
        stage('Code') {
            steps {
                echo 'Fetching the code'
            }
        }
        
        stage('Build') {
            steps {
                echo 'building the code'
            }
        }
        
        stage('Push to docker hub') {
            steps {
                echo 'pushing to docker hub'
            }
        }
        
        stage('Deploy') {
            steps {
                echo 'Deploying the container '
            }
        }
    }
}
