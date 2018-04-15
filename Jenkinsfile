pipeline {
  agent any
  stages {
    stage('hi') {
      steps {
        echo 'hi!'
      }
    }
    stage('build') {
      steps {
        sh '''mvn clean install
'''
      }
    }
    stage('test') {
      steps {
        fileExists 'Test123-0.0.1-SNAPSHOT.jar'
      }
    }
  }
}