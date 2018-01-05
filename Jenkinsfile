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
            
            build(job: 'nonesiste', quietPeriod: 2)
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