pipeline {
  agent {
    node {
      label 'docker'
    }

  }
  stages {
    stage('test') {
      parallel {
        stage('Test') {
          steps {
            echo 'testing'
          }
        }

        stage('parallel') {
          steps {
            echo 'parallel'
          }
        }

      }
    }

    stage('Build') {
      steps {
        echo 'building '
      }
    }

    stage('Clean up') {
      steps {
        echo 'cleaning'
      }
    }

  }
}