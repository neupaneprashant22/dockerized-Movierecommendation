pipeline {
    agent any

    stages {
        stage('SCM Checkout') {
            steps{
            git 'https://github.com/neupaneprashant22/dockerized-Movierecommendation'
            }
        }
        stage('Build docker image') {
            steps {  
               sh 'echo Build docker image '
               sh 'pwd' 
            }
        }
        // stage('Run docker container') {
        //     steps {
        //         sh 'docker-compose up'
        //     }
        // }
    }
}
