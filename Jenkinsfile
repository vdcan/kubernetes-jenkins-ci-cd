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
    stage('Docker Push') {
      steps {
        echo 'Pushing to Docker Registry...'
      }
    }
    stage('SonarQube') {
      steps {
        echo 'Uploading to Sonar...'
        sh '''mvn sonar:sonar \\
  -Dsonar.host.url=http://52.226.67.67 \\
  -Dsonar.login=5c965226d12f03ad373ae5d7ad2b660d52839123'''
      }
    }
    stage('Kubernetes') {
      steps {
        echo 'Updating Kubernetes resources...'
      }
    }
  }
}