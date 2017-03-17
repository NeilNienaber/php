#!groovy

pipeline {
  sh 'echo TEST'
  sh 'mkdir test'
  agent { docker 'php' }
  stages {
    stage('build') {
      steps {
        sh 'php --version'    
      }
    }
  }
}
