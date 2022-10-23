pipeline{
    agent any
    stages {

        stage('Build Docker Image'){
            steps{
                script{
                    dockerapp = docker.build("shuzito/kube-news:${env.BUILD_ID}", '-f ./src/dockerfile ./src')
                }
            }
        }
    }
}
