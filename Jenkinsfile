pipeline {
  agent any
  stages {
    stage('Stage1') {
      steps {
        waitUntil() {
          echo 'Hello'
          return true
        }   
      }
    }
    stage('Stage2') {
      steps {
        echo 'World'
      }
    }
  }
  triggers {
    cron('* * * * *')
  }
}
