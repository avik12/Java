pipeline{
  agent any
  ENVIORMENT {
    bnch = "${BRANCH_NAME}"
  }
  stages{
    stage("Test"){
      steps{
          echo "Hello  Testing"
        }
      }
    stage("Branch Wise Test"){
      when {
        expression {
         "$bnch"  == "master"
          }
        }
      steps{
        echo "Hello Master"
      }
    }
  }
}
