#!groovy

  node {
    sh '''#!/bin/bash -l
      echo $0
      echo TEST
      mkdir test
      mkdir -p /root/meh
    '''
    docker.image('php:5.6').withRun {c ->
      sh '''#!/bin/bash -l
        echo $0
        apt-get update -yqq
        apt-get install git -yqq
        curl -sS https://getcomposer.org/installer | php
        php composer.phar install
      '''
    }                                                                                      
  }
