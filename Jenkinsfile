pipeline {
    agent any
    options {
            skipStagesAfterUnstable()
    }
    stages {
        stage('Build') {
            steps {
                git 'https://github.com/shadowhijackers/jenkins-angular.git'
                sh "npm i"
                sh "sudo ng build --prod"
            }
        }
    }
}
