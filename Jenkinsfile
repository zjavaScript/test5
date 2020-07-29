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
        timeout(time: 10, unit: 'MINUTES') {
          timeout(time: 20) {
            timeout(time: 30) {
              timeout(time: 40) {
                timeout(time: 50) {
                  timeout(time: 60) {
                    timeout(time: 70) {
                      timeout(time: 80)
                    }

                  }

                }

              }

            }

          }

        }

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

    stage('f') {
      steps {
        echo '1111111'
      }
    }

  }
}