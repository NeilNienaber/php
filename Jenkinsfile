#!groovy

  node {
    sh 'echo TEST'
    sh 'mkdir test'
    sh 'mkdir -p /root/meh'
    docker.image('php').inside {
      sh 'ls -la'
    }                                                                                        
  }
