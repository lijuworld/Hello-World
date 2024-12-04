pipeline {
    agent any

    stages {
        stage('Code') {
            steps {
                echo 'Clone the code'
                git url:"https://github.com/lijuworld/Hello-World.git" ,branch:"main"
            }
        }
        
        stage('Build') {
            steps {
                echo 'building the code'
                //bat "docker build -t hello-world ."
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
		sh 'kubectl apply -f nginx-deployment.yaml'
            }
        }
    }
}
