#!groovy

  node {
    sh 'echo TEST'
    sh 'mkdir test'
    sh 'mkdir -p /root/meh'
    docker.image('php').withRun {c ->
      sh 'echo TEST'
    }                                                                                      
  }
