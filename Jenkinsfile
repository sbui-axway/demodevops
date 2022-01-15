pipeline {
  agent {
    docker {
      image 'stoplight/spectral'
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