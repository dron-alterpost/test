pipeline {
  agent any
  stages {
    stage('VCS') {
      parallel {
        stage('Sleep 1') {
          steps {
            sh 'cat README.md'
            sleep 30
          }
        }
        stage('Sleep 2') {
          steps {
            sleep 35
          }
        }
      }
    }
  }
}