pipeline {
  agent {
    node {
      label 'mesos-production'
    }
    
  }
  stages {
    stage('Setup') {
      steps {
        sh 'docker run -e "COMMIT_HASH=origin/tests-passed" -e SKIP_JS    discourse/discourse_test:release'
      }
    }
  }
}