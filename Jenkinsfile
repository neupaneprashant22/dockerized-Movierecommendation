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
               sh ' docker-compose --version '
            }
        }
    }
    post {
    failure {
        mail to: 'neupaneprashant22@gmail.com',
             subject: "Failed Pipeline:",
             body: "Something is wrong with pipeline"
    }
    success {
        mail to: 'neupaneprashant22@gmail.com',
             subject: "Pipeline Build:",
             body: "Pipeline is build"
    }
}
}
