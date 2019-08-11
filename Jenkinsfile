node {
        stage("----- Checkout -----") {
            git 'https://github.com/shadowhijackers/jenkins-angular.git'
        }

        stage("----- Preparation -----"){
             sh "npm i"
        }

        stage("----- Build ----------") {
                sh "sudo ng build --prod"
        }

}
