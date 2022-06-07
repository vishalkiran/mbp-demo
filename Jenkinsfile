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

  stage("Sonar Analysis"){
      when {
        branch 'develop'
      }
      steps{
        echo "Sonar Analysis"
  }

  stage("Deploy to dev and test"){
      when {
        branch 'develop'
      }
      steps{
        echo "Deploy to dev"
         echo "Deploy to test"
  }

  stage("Deploy to UAT"){
      when {
        branch 'uat'
      }
      steps{
        print "Deploy to UAT..."
  }

  stage("Deploy Prod"){
      when {
        branch 'master'
      }
      steps{
        print "Deploy to prod..."
      }
}
