pipeline {
  agent {
    node {
      label 'mesos-production'
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