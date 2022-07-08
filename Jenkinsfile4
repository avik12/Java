pipeline{
  agent any
  stages{
    stage("Test"){
      steps {
          echo "Hello  Testing"
        }
      }
    }
  post {
    always {
      echo 'ALways'
      }
    success {
      echo 'Success'
      }
    failure {
      echo 'Failure'
    }
    unstable {
      echo 'Unstable'
    }
  }
}
