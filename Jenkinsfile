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
        sh 'spectral lint crm.openapi.yml'
      }
    }

  }
}