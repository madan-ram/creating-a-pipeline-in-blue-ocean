pipeline {
  agent any
  stages {
    stage('docker') {
      steps {
        sh 'docker run -p 3000:3000 node:6-alpine '
      }
    }
    stage('build') {
      steps {
        sh 'npm install'
      }
    }
  }
}