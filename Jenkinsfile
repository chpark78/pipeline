pipeline {
  agent any
  stages {
    stage('Stage1') {
      steps {
        echo 'Hello'
        waitUntil() {
          flag = true
          flag
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
