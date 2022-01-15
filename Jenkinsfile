pipeline {
  agent {
    docker {
      image 'spectral:latest'
    }
  }
  stages {
    stage('validate') {
     
      steps {
        sh 'spectral lint crm.openapi.yml'
      }
    }

  }
}