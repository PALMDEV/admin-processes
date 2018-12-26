pipeline {
  agent {
    docker {
      image 'asd'
      args '''
asd'''
    }

  }
  stages {
    stage('Build') {
      steps {
        sh 'echo "hey"'
      }
    }
  }
}