pipeline {
  agent any
  stages {
    stage('a') {
      parallel {
        stage('a') {
          steps {
            sh 'ls'
          }
        }

        stage('b') {
          steps {
            sh 'ls'
          }
        }

      }
    }

    stage('c') {
      steps {
        sh 'ls'
      }
    }

    stage('d') {
      parallel {
        stage('d') {
          steps {
            sh 'ls'
          }
        }

        stage('e') {
          steps {
            sh 'ls'
            echo '123'
          }
        }

      }
    }

  }
}