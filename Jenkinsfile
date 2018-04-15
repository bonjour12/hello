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
        sh '''#!/bin/bash
mvn clean install
'''
      }
    }
  }
}