pipeline {
  agent any
  stages {
    stage('serial01') {
      steps {
        echo 'Tokyo central city is'
      }
    }
    stage('parallel') {
      steps {
        parallel(
          "sleep": {
            sleep 10
          },
          "echo01": {
            echo 'paralell paralell'
          },
          "echo02": {
            echo 'paralell paralell'
          },
          "echo03": {
            echo 'paralell paralell'
          },
          "echo04": {
            echo 'world'
          }
        )
      }
    }
    stage('serial02') {
      steps {
        echo 'end'
      }
    }
  }
}
