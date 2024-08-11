pipeline {
  agent any
  stages {
    stage('Plan') {
      steps {
        echo 'To plan the app dev'
      }
    }

    stage('code') {
      steps {
        echo 'devloper devlop the code'
      }
    }

    stage('build') {
      parallel {
        stage('build') {
          steps {
            echo 'the code should be build'
          }
        }

        stage('test') {
          steps {
            echo 'the code should be tested'
          }
        }

        stage('deploy') {
          steps {
            echo 'code should be deployed'
          }
        }

        stage('operate') {
          steps {
            echo 'the code should be operated'
          }
        }

      }
    }

  }
}