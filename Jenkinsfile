pipeline {
    agent any

    stages {

        stage ('Build Docker Image') {
            steps {
                script {
                    dockerapp = docker.build("jehmes/kube-news:${env.BUILD_ID}", "--file ./src/Dockerfile ./src")
                }
            }
        }

    }
}