pipeline {
  agent any
  stages {
    stage('Stage1') {
      steps {
        waitUntil() {
          echo 'Hello'
          def result = 0
          return (result == 0)
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
