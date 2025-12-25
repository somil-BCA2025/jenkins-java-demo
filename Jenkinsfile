pipeline {
  agent any 

  stages{
    stage('checkout') {
      steps {
        echo 'Code already checkout by Jenkins'
      }
    }

      stage('Build') {
        steps {
          bat 'mv clean package'
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
} 
