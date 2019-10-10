pipeline {
  agent { label 'nodejs-app' }
  stages {
    stage('SayHello') {
      agent { label 'nodejs-app' }
      steps {
        echo 'Hello World'
        sh 'java -version'
        }
      }
    }
  }
