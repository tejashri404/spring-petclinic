pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'echo \'Building\''
      }
    }

    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            echo 'echo \'Testing\''
          }
        }

        stage('Api_Test') {
          steps {
            echo 'API Test'
          }
        }

      }
    }

    stage('Archive') {
      steps {
        echo 'echo \'Archiving\''
      }
    }

  }
}