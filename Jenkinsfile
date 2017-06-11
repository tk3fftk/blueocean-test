pipeline {
  agent { docker 'node:8' }
  tools { docker 'docker' }
  stages {
    stage('echo') {
      steps {
        echo '`node -v`'
      }
    }
  }
}
