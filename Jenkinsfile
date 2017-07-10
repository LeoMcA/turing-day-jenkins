pipeline {
  agent {
    docker {
      image 'discourse/discourse_dev:release'
    }
    
  }
  stages {
    stage('Setup') {
      steps {
        sh '''ls .
ls ../'''
        git(url: 'https://github.com/discourse/discourse.git', branch: 'tests-passed')
        sh '''ls .
ls ../'''
      }
    }
  }
}