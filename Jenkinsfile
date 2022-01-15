pipeline {
  agent {
    docker {
      image 'node:16.13.1-alpine'
    }

  }
  stages {
    stage('lint') {
      steps {
        sh '''npm config set unsafe-perm true
npm install -g --unsafe-perm spectral'''
        sh 'spectral --h'
      }
    }

  }
}