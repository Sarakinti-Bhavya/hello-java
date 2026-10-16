pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo 'Source code will be checked out from GitHub'
            }
        }

        stage('Build') {
            steps {
                sh 'mvn clean package'
            }
        }
    }
}
