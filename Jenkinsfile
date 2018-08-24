pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            bat 'echo hello'
            bat 'echo hellohi'
          }
        }
        stage('Build1') {
          steps {
            bat 'echo build1'
          }
        }
      }
    }
    stage('test') {
      steps {
        bat 'echo test'
      }
    }
  }
  environment {
    Name = 'test'
  }
}