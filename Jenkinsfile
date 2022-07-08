pipeline{
  agent { docker{ image 'openjdk:11-jdk-slim'}}
  stages{
    stage("Check Version"){
      steps{
          sh 'mvn --version'
      }
    }
  }
}
