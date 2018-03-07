pipeline {
  agent any
  stages {
    stage('VCS') {
      steps {
        sh 'cat README.md'
        git(poll: true, changelog: true, url: 'git@github.com:dron-alterpost/test.git', branch: 'master')
      }
    }
    stage('Prompt') {
      steps {
        input 'Finished using the web site?'
      }
    }
  }
}