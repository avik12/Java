pipeline{
  agent any
  stages{
    stage("Test"){
      steps{
          echo "Hello  Testing"
        }
      }
    stage("Test"){
      when {
        expression {
            BRANCH_NAME == "master"
          }
        }
      steps{
        echo "Hello Master"
      }
    }
  }
}
