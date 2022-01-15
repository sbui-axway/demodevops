pipeline {
  agent {
    docker {
      image 'node:16.13.1-alpine'
    }

  }
  stages {
    stage('validate') {
      steps {
        sh 'yarn global add @stoplight/spectral-cli'
        sh 'spectral lint crm.openapi.yml'
      }
    }

  }
}