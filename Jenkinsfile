pipeline {
  agent {
    docker { image 'python:3.11-slim' }
  }
  stages {
    stage('Checkout') {
      steps { checkout scm }
    }
    stage('Build/Test') {
      steps {
        sh 'python --version'
        sh 'python hello.py'
      }
    }
  }
}
