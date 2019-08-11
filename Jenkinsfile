pipeline {
    agent any
    options {
            skipStagesAfterUnstable()
    }
    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/shadowhijackers/jenkins-angular.git'
            }
        }
        stage('Prepare') {
            steps {
               sh "npm i"
            }
        }
        stage('Build') {
            steps {
               sh "sudo ng build --prod"
            }
        }
    }
}
