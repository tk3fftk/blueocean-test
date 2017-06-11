pipeline {
  agent any
  stages {
    stage('sleep') {
      steps {
        parallel(
          "sleep": {
            sleep 10
            
          },
          "": {
            echo 'aaaa'
            
          }
        )
      }
    }
    stage('echo') {
      steps {
        echo 'hogehoge'
      }
    }
  }
}