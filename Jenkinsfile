pipeline {
  agent {
    docker {
      image 'mvn'
    }

  }
  stages {
    stage('Build') {
      steps {
        sh '''mvn build
'''
      }
    }
    stage('Test') {
      steps {
        sh '''mvn test
'''
      }
    }
    stage('Deploy') {
      steps {
        sh '''./Deploy
'''
      }
    }
  }
}