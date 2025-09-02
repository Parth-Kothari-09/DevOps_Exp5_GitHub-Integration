pipeline {
  agent {
    docker {
      image 'python:3.11-slim'
      // reuseNode true  // optional
    }
  }
  stages {
    stage('Checkout') { steps { checkout scm } }
    stage('Build/Test') {
      steps {
        sh 'python --version'
        sh 'python hello.py'
      }
    }
  }
}
