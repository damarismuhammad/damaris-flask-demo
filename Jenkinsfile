pipeline {
  agent any
  stages {
    stage('Pull') {
       checkout scm     
    }

    stage('Build') {
      steps {
        sh 'echo "hello ini pipeline"'
      }
    }

  }
  environment {
    APP_ENV = 'production'
  }
}