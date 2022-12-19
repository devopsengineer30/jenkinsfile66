pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'I want to Build'
      }
    }

    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            echo 'I want to Print'
          }
        }

        stage('Deploy') {
          steps {
            echo 'Deployed'
          }
        }

      }
    }

  }
}