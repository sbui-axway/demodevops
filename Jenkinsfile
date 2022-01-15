pipeline {
  agent {
    docker {
      image 'stoplight/spectral'
    }

  }
  stages {
    stage('lint') {
      steps {
        sh 'spectral -h'
      }
    }

  }
}