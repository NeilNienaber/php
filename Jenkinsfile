#!groovy

node {
  deleteDir()
  step([$class: 'GitHubSetCommitStatusBuilder'])
  docker.image('php:5.6').inside {
    `checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: '4d983e5d-96b4-41fc-93ec-618c8c519e4f', url: 'git@github.com:NeilNienaber/php.git']]])
  }
}
