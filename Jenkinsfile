pipeline {
  agent any
  stages {
    stage('Pull') {
      steps {
        git(credentialsId: 'damaris-ssh-project', url: 'git@github.com:damarismuhammad/damaris-flask-demo.git', branch: 'main')
      }
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