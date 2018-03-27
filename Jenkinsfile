pipeline {
  agent any
  stages {
    stage('Checkout') {
      steps {
        git 'https://github.com/hijmenfokker/kubernetes-jenkins-ci-cd.git'
      }
    }
    stage('Build & Unit Test') {
      steps {
        echo 'Not implemented'
      }
    }
    stage('Docker build') {
      steps {
        echo 'Building Docker image...'
      }
    }
  }
}