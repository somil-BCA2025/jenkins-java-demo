pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo 'Code already checked out by Jenkins'
            }
        }

        stage('Build') {
            steps {
                sh 'mvn clean package'
            }
        }
    }

    post {
        success {
            echo 'Build Successfully'
        }
        failure {
            echo 'Build Failed'
        }
        always {
            echo 'This Always Runs'
        }
    }
}

