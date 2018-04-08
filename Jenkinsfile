pipeline {
  agent any
  stages {
    stage('docker') {
      steps {
        sh 'docker run node:6-alpine -p 3000:3000'
      }
    }
    stage('build') {
      steps {
        sh 'npm install'
      }
    }
  }
}