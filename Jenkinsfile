Jenkinsfile (Declarative Pipeline)
pipeline {
    agent any

    stages {
        stage('SCM Checkout') {
            steps{
            git 'https://github.com/ravdy/nodejs-demo.git'
            }
        }
        stage('Build docker image') {
            steps {  
                sh 'docker-compose build'  
            }
        }
        }
        stage('Run docker container') {
            steps {
                sh 'docker-compose up'
            }
        }
    }
