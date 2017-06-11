pipeline {
  agent any
  stages {
    stage('echo') {
      steps {
        echo 'hogehoge'
        script {
            def browsers = ['chrome', 'firefox']
            for (int i = 0; i < browsers.size(); ++i) {
                echo "Testing the ${browsers[i]} browser"
            }
        }
      }
    }
    stage('if-else') {
      steps {
        script {
          if (env.BRANCH_NAME == 'master') {
              echo 'It's master branch'
          } else {
              echo 'It's not master branch'
          }
        }
      }
    }
    stage('try-catch') {
      steps {
        script {
          try {
              sh 'exit 1'
          }
          catch (exc) {
              echo 'Something failed, I should sound the klaxons!'
              throw
          }
        }
      }
    }
  }
}
