pipeline {
  agent any
  stages {
    stage('dev') {
      steps {
        echo 'this is dev stage'
      }
    }

    stage('build') {
      steps {
        echo 'this is build stage'
      }
    }

    stage('test') {
      steps {
        echo 'this is test stage'
      }
    }

    stage('UAT') {
      parallel {
        stage('UAT') {
          steps {
            echo 'this is UAT stage'
          }
        }

        stage('deploy') {
          steps {
            echo 'this is deploy stage'
          }
        }

        stage('operate') {
          steps {
            echo 'this is operate stage'
          }
        }

      }
    }

  }
}