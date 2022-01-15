pipeline {
  agent {
    docker {
      image 'node:16.13.1-alpine'
    }

  }
  stages {
    stage('lint') {
      steps {
        sh 'npm install -g spectral'
        sh 'spectral --h'
      }
    }

  }
}