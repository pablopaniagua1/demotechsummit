pipeline {
  agent {
    node {
      label 'a'
    }

  }
  stages {
    stage('Download git code') {
      steps {
        git(url: 'https://github.com/pablopaniagua1/demotechsummit.git', branch: 'master')
      }
    }

    stage('Generate Build for Power') {
      parallel {
        stage('Generate Build for Power') {
          steps {
            echo 'hihi'
          }
        }

        stage('Generate build for Z') {
          steps {
            echo 'Hi'
          }
        }

      }
    }

    stage('Deploy in Power') {
      parallel {
        stage('Deploy in Power') {
          steps {
            echo 'Deploy'
          }
        }

        stage('') {
          steps {
            echo 'deploy in Z'
          }
        }

      }
    }

    stage('Test') {
      steps {
        sleep 1
      }
    }

  }
}