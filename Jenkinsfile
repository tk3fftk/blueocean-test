pipeline {
  agent { docker 'node:8' }
  stages {
    stage('echo') {
      steps {
        echo '`node -v`'
      }
    }
  }
}
