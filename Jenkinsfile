pipeline {
  agent {
    dockerfile {
      filename 'Dockerfile'
    }
    
  }
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