pipeline{
  agent any
  environment {
    bnch = "${BRANCH_NAME}"
    id = "${JOB_BASE_NAME}"
  }
  parameters {
  booleanParam (description: 'OS', name: 'OsBuild')
  choice (choices: ['UAT', 'SIT', 'DEV'], description: 'Build Environment ', name: 'Env')
  string (defaultValue: 'Demo', description: 'NameOfJob', name: 'JobName')
}
  stages{
    stage("Test"){
      steps{
          echo "Hello  Testing"
          echo "${id}"
        }
      }
    stage("Test1"){
      steps{
        script{
         if (params.Env == 'UAT'){
            echo params.Env
         }
          else {
            echo "Not If "
          }
        }
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
