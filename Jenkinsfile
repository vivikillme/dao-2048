pipeline {
  agent any
  stages {
    stage('build') {
      parallel {
        stage('build') {
          steps {
            echo 'hello world'
          }
        }
        stage('build2') {
          steps {
            emailext(subject: 'test build', body: 'ok', to: 'liuruiey@gmail.com')
          }
        }
      }
    }
  }
}