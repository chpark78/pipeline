pipeline {
  agent any
  stages {
    stage('Stage1') {
      steps {
        echo 'Hello'
        waitUntil() {
          sh 'exit 0'
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