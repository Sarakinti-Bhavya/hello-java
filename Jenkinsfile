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
        
        
        stage('Test') {
    steps {
        echo 'Running tests...'
        sh 'exit 1'
    }
}
    }
      post {
        success {
            echo 'Pipeline completed successfully!'
        }

        failure {
            echo 'Pipeline failed!'
        }

        always {
            echo 'Pipeline execution finished.'
        }
    }
}
