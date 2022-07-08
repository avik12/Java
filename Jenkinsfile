pipeline{
  agent any
  stages{
    stage("Check Version"){
      steps{
        retry(3){
        sh './health-check.sh'
        }
      }
    }
  }
}
