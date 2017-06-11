pipeline {
  agent any
  stages {
    stage('sleep') {
      steps {
        sleep 10
      }
    }
    stage('echo') {
      withNPM(npmrcConfig:'') {
        steps {
          sh 'npm install'
          sh 'node -v'
        }
      }
    }
  }
}
