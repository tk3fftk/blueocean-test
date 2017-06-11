pipeline {
  agent { docker 'node:8' }
  stages {
    stage('sleep') {
      steps {
        sleep 10
      }
    }
    stage('echo') {
      steps {
        echo '`node -v`'
      }
    }
  }
}
