pipeline {
  agent any
  stages {
    stage('stage1') {
      steps {
        echo 'ls'
      }
    }
    stage('stage2') {
      steps {
        echo 'branch'
        withPythonEnv(pythonInstallation: 'test')
      }
    }
  }
}