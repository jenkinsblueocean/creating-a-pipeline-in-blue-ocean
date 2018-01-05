pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            catchError() {
              script {
                start = new Date()
                echo 'prova ${start}'
                build 'nonesiste'
              }
            }
          }
        }
        stage('Stage 2 parallel') {
          steps {
            echo 'stage 2 parallel'
          }
        }
      }
    }
    stage('Stage 3 serial') {
      steps {
        echo 'stage 3 serial'
      }
    }
  }
}
