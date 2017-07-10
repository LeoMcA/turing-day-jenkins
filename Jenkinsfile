pipeline {
  agent any
  stages {
    stage('Setup') {
      steps {
        git(url: 'https://github.com/discourse/discourse.git', changelog: true, branch: 'tests-passed')
        sh 'ls .'
      }
    }
  }
}