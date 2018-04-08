pipeline {
  agent any
  stages {
    stage('docker') {
      steps {
        sh '''docker run \\
-u root \\
-p 3000:3000 \\
-v /Users/madanram/SoulOfCoder/jenkins-data:/var/jenkins_home \\
-v /var/run/docker.sock:/var/run/docker.sock \\
-it node:6-alpine sh '''
      }
    }
    stage('build') {
      steps {
        sh 'npm install'
      }
    }
  }
}