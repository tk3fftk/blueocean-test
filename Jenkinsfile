pipeline {
  node {
      stage('if-else') {
        if (env.BRANCH_NAME == 'master') {
            echo 'It is master branch'
        } else {
            echo 'It is not master branch'
        }
      }
      stage('try-catch') {
        try {
            sh 'exit 1'
        }
        catch (exc) {
            echo 'Something failed, I should sound the klaxons!'
        }
      }
  }
}
