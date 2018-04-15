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
        sh 'mvn clean install'
      }
    }
  }
}