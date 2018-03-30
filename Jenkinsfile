pipeline {
  agent any
  stages {
    stage('Stage1') {
      steps {
        echo 'Hello'
        waitUntil() {
          sh 'wget http://www.naver.com'
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