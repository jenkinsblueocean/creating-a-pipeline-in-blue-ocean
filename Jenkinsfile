pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            catchError() {
              echo 'prova'
            }
            
          }
        }
        stage('Build 2') {
          steps {
            catchError() {
              echo 'prova build2'
            }
            
          }
        }
      }
    }
  }
}