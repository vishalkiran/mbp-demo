pipeline {
  agent any

  stages{
    stage("Maven build"){
      when {
        branch 'develop'
      }
      steps{
        sh "mvn clean package"
      }
    }
  }
}