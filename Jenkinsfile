pipeline {
  agent any
  stages {
    stage('Dev') {
      steps {
        echo 'this is dev stage'
      }
    }

    stage('built') {
      steps {
        echo 'this is built stage'
      }
    }

    stage('test') {
      parallel {
        stage('test') {
          steps {
            echo 'this is testing stage'
          }
        }

        stage('test1') {
          steps {
            echo 'first stage testing'
          }
        }

        stage('test2') {
          steps {
            echo 'second stage testing'
          }
        }

      }
    }

  }
}