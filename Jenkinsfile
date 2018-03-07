pipeline {
  agent any
  stages {
    stage('VCS') {
      steps {
        sh 'cat README.md'
      }
    }
    stage('Prompt') {
      steps {
        input 'Finished using the web site?'
      }
    }
  }
}