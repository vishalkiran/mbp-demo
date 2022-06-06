pipeline {
  agent any

  tools {
    maven 'Maven-3.8.5'
  }

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