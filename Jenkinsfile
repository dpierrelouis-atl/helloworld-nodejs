pipeline {
  agent { label 'nodejs-app' }
  options { 
    buildDiscarder(logRotator(numToKeepStr: '2'))
    skipDefaultCheckout true
  }
  stages {
    stage('SayHello') {
      agent { label 'nodejs-app' }
      steps {
        container('nodejs') {
          echo 'Hello World'
          sh 'node --version'
          }
        }
      }
    stage('Build and Push Image') {
      when {
         beforeAgent true
         branch 'master'
      }
      steps {
         echo "TODO - build and push image"
      }
    }
  }
}
