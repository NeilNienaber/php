#!groovy

node {
  
  stage('Configure') {
    deleteDir()
  }

  stage('Checkout') {
    checkout scm
  }
  
  stage('Dockerer') {
    docker.image('php:5.6').inside {
      sh 'echo HELP'
    }
  }
}
