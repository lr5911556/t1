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
    stage('gethost') {
      steps {
        sh 'hostname'
      }
    }
    stage('cathosts') {
      parallel {
        stage('cathosts') {
          steps {
            sh 'cat /etc/hosts'
          }
        }
        stage('cat') {
          steps {
            sh 'cat /etc/hosts'
          }
        }
      }
    }
    stage('') {
      steps {
        sh 'python --version'
      }
    }
  }
}