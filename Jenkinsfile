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
                sh 'cd /home/app/'
                sh 'docker-compose build'  
            }
        }
        stage('Run docker container') {
            steps {
                sh 'cd /home/app/'
                sh 'git clone https://github.com/neupaneprashant22/dockerized-Movierecommendation.git'
                sh 'docker-compose up'
            }
        }
    }
}
