pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            bat 'echo %name%'
          }
        }

        stage('Build2') {
          steps {
            bat 'echo Build2'
          }
        }

      }
    }

    stage('Test') {
      steps {
        bat 'echo %name%'
        bat 'echo Test'
      }
    }

  }
  environment {
    Name = 'FirstStone'
  }
}