pipeline {
  agent any
  stages {
    stage('Setup') {
      steps {
        sh '''docker run
    -e "COMMIT_HASH=origin/tests-passed"
    -e SKIP_JS=1
    discourse/discourse_test:release'''
      }
    }
  }
}