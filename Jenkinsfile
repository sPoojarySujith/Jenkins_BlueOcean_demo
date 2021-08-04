pipeline {
  agent {
    node {
      label 'agent1'
    }

  }
  stages {
    stage('Build') {
      steps {
        echo 'Building'
      }
    }

    stage('Test1') {
      parallel {
        stage('Test1') {
          steps {
            echo 'Test 1 successful'
          }
        }

        stage('Test2') {
          steps {
            echo 'Test2 Successful'
          }
        }

        stage('Test3') {
          steps {
            echo 'Test3 Successful'
            sh 'dddd'
          }
        }

        stage('Test4') {
          steps {
            echo 'Test4 Successful'
          }
        }

      }
    }

    stage('Deploy1') {
      parallel {
        stage('Deploy1') {
          steps {
            echo 'Deploy1 Successful'
          }
        }

        stage('Deploy2') {
          steps {
            echo 'Deploy2 Successful'
          }
        }

        stage('Deploy3') {
          steps {
            echo 'Deploy3 Successful'
          }
        }

      }
    }

    stage('Release') {
      steps {
        echo 'Release Job Success!!!'
      }
    }

  }
}