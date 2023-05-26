pipeline {
  agent any
  stages {
    stage('Pull') {
       steps {
        node ('master') {
          checkout scm
        } 
      }     
    }

    stage('Build') {
      steps {
        node ('master') {
          sh 'echo "hello ini pipeline"'
        }
      }
    }

  }
  environment {
    APP_ENV = 'production'
  }
}