pipeline {
  agent any
  stages {
    stage('t1') {
      parallel {
        stage('t1') {
          steps {
            sh 'java -version'
          }
        }
        stage('t2') {
          steps {
            sh 'java -version'
          }
        }
      }
    }
    stage('') {
      steps {
        sh 'hostname'
      }
    }
  }
}