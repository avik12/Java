pipeline{
  agent any
  environment {
    bnch = "${BRANCH_NAME}"
    id = "${JOB_BASE_NAME}"
  }
  stages{
    stage("Test"){
      steps{
          echo "Hello  Testing"
        echo "${id}"
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
