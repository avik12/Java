def gv
pipeline{
  agent any
   stages{
    stage("Test"){
      steps{
        script{
          gv = load "script.groovy"
          }
        }
      }
    stage("Test1"){
      steps{
        script{
          gv.buildApp()
        }
      }
    }
   }
}
