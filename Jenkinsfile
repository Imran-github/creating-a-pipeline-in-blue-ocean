pipeline {
  agent none
  stages {
    stage('Build') {
      agent {
        docker {
          image 'node:6-alpine'
          args '-p 3000:3000'
        }

      }
      steps {
        sh 'sudo npm install'
      }
    }

  }
}