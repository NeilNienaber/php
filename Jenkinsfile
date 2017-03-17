#!groovy

  node {
    sh '''
      echo TEST
      mkdir test
      mkdir -p /root/meh
    '''
    docker.image('php:5.6').withRun {c ->
      sh 'echo TEST'
    }                                                                                      
  }
