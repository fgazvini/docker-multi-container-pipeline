pipeline {
  agent none
  stages {
    stage('Maven-container-backend') {
      agent {
        docker {
          image 'maven:3-alpine'
        }
        
      }
      steps {
        sh 'mvn --version'
      }
    }
    stage('Frontend-NodeJS-Container') {
      agent {
        docker {
          image 'node:7-alpine'
        }
        
      }
      steps {
        sh 'node --version'
      }
    }
  }
}