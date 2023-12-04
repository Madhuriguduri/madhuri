pipeline {
  agent any
  stages {
    stage('build') {
      parallel {
        stage('build') {
          steps {
            echo 'this is build'
          }
        }

        stage('adding') {
          steps {
            echo 'build is adding'
          }
        }

        stage('code') {
          steps {
            echo 'build code'
          }
        }

      }
    }

    stage('develop') {
      parallel {
        stage('develop') {
          steps {
            echo 'develop the build '
          }
        }

        stage('implement') {
          steps {
            echo 'impliment'
          }
        }

      }
    }

    stage('test') {
      steps {
        echo 'test the code'
      }
    }

    stage('impliment') {
      steps {
        echo 'impliment the code'
      }
    }

  }
}