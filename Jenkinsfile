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
      parallel {
        stage('test') {
          steps {
            fileExists 'Test123-0.0.1-SNAPSHOT.jar'
          }
        }
        stage('test2') {
          steps {
            echo 'tes t2'
          }
        }
      }
    }
    stage('package') {
      steps {
        sh '''mvn clean package
'''
      }
    }
  }
}