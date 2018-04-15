pipeline {
  agent any
  stages {
    stage('hi') {
      steps {
        echo 'hi!'
      }
    }
    stage('tmp') {
      steps {
        pwd(tmp: true)
      }
    }
  }
}