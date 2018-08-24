pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            bat 'echo hello'
            bat 'cd \\Users\\1021534\\Dektop\\Jenkins\\hello.py'
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