pipeline {
  agent any
  stages {
    stage('sleep') {
      steps {
        sleep 10
      }
    }
    stage('echo') {
      steps {
        sh 'npm install'
        sh 'node -v'
      }
    }
  }
}
