pipeline {
  agent {
    docker {
      image 'stoplight/spectral'
    }

  }
  stages {
    stage('lint') {
      steps {
        sh 'lint crm.openapi.yml'
      }
    }

  }
}