pipeline{
  agent any
  environment {
    bnch = "${BRANCH_NAME}"
  }
  stages{
    stage("Test"){
      steps{
          echo "Hello  Testing"
        echo "${bnch}"
        }
      }
    stage("Branch Wise Test"){
      when {
        expression {
          "${bnch}"  == "master"
          }
        }
      steps{
        echo "Hello Master"
      }
    }
  }
}
