pipeline {
  agent any
  stages {
    stage('Checkout') { steps { checkout scm } }
    stage('Build/Test') {
      steps {
        sh '''
          set -e
          if ! command -v python3 >/dev/null 2>&1; then
            apt-get update
            apt-get install -y python3
          fi
          python3 --version
          python3 hello.py
        '''
      }
    }
  }
}
