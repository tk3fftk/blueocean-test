pipeline {
  agent any
  stages {
    stage('sleep') {
      steps {
        sleep 10
      }
    }
    stage('echo') {
      withNPM() {
        steps {
          sh 'npm install'
          sh 'node -v'
        }
      }
    }
  }
}
