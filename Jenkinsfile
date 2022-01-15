pipeline {

  stages {
    stage('validate') {
      agent {
        docker {
          image 'spectral:latest'
        }
      }
      steps {
        sh 'spectral lint crm.openapi.yml'
      }
    }

  }
}