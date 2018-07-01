pipeline {
  agent any
  stages {
    stage('stage1') {
      parallel {
        stage('stage1') {
          steps {
            timestamps() {
              sh 'ls -ltr'
            }

          }
        }
        stage('stage2') {
          agent {
            node {
              label 'normalSlave'
            }

          }
          steps {
            echo 'stage2'
          }
        }
      }
    }
  }
}