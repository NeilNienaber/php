#!groovy

  node {
    sh '''
      echo TEST
      mkdir test
      mkdir -p /root/meh
    '''
    docker.image('php:5.6').withRun {c ->
      sh '''
        apt-get update -yqq
        apt-get install git -yqq
        docker-php-ext-install pdo_mysql
        curl -sS https://getcomposer.org/installer | php
        php composer.phar install
      '''
    }                                                                                      
  }
