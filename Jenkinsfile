pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh 'npm install'
      }
    }
  }
  environment {
    agent = 'docker'
  }
}