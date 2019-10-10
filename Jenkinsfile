pipeline {
  agent { label 'nodejs-app' }
  stages {
    stage('SayHello') {
      agent { label 'nodejs-app' }
      steps {
        container('nodejs') {
          echo 'Hello World'
          sh 'java -version'
          }
        }
      }
    }
  }
