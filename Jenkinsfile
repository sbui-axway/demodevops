pipeline {
  agent {
    docker {
      image 'node:16.13.1-alpine'
    }

  }
  stages {
    stage('validate') {
      agent {
                docker { image 'stoplight/spectral' }
            }
      steps {
        sh 'npm install  spectral'
        sh 'spectral --h'
      }
    }

  }
}