pipeline {
  agent any
  stages {
    stage('Stage1') {
      steps {
        echo 'Hello'
        waitUntil() {
          sh 'curl http://www.naver.com'
          true
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
