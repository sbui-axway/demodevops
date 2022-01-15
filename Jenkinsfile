pipeline {
  agent {
    docker {
      image 'stoplight/spectral'
      args 'entrypoint: [""]'
    }

  }
  stages {
    stage('lint') {
      steps {
        sh 'spectral lint crm.openapi.yml'
      }
    }

  }
}