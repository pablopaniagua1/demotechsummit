pipeline {
  agent any
  stages {
    stage('test') {
      parallel {
        stage('test') {
          steps {
            sh 'sh "echo hello"'
          }
        }

        stage('test2') {
          steps {
            sh 'sh "echo hello"'
          }
        }

      }
    }

    stage('end') {
      steps {
        sh 'sh "echo test"'
      }
    }

  }
  environment {
    test = 'test'
  }
}