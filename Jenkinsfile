pipeline {
  agent any
  stages {
    stage('Checkout') {
      steps { checkout scm }
    }
    stage('Build/Test') {
      steps {
        sh 'python3 --version || python --version'
        sh 'echo Running pipeline...'
      }
    }
  }
}
