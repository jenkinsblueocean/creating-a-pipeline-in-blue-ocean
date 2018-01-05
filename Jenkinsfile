pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        catchError() {
          echo 'prova'
          build 'nonesiste'
        }
        
      }
    }
  }
}