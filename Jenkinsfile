pipeline{
  agent any
  stages{
    stage("Check Version"){
      steps{
        retry(3){
        sh 'chmod 755 health-check.sh'   
        sh './health-check.sh'
        }
      }
    }
  }
}
