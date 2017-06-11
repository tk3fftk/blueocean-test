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
  }
}
