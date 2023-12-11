pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                git 'https://github.com/MotebAlhrbi/eCommerce-Application'
                script {
                    def mvnHome = tool 'Maven'
                    def mvnCMD = "${mvnHome}/bin/mvn"
                    sh "${mvnCMD} clean install"
                }
            }
        }
    }

    // Add more stages for testing, deployment, etc.
}
