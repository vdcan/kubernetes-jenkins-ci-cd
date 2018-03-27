pipeline {
  agent any
  stages {
    stage('Checkout') {
      steps {
        git 'https://github.com/hijmenfokker/kubernetes-jenkins-ci-cd.git'
      }
    }
    stage('Maven Build') {
      steps {
        echo 'Not implemented'
      }
    }
    stage('Docker Build') {
      steps {
        echo 'Building Docker image...'
      }
    }
  }
}