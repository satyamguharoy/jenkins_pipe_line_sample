pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            echo 'Build stage'
          }
        }
        stage('Build Parallel') {
          steps {
            echo 'Building Parallel'
          }
        }
      }
    }
    stage('Test') {
      steps {
        echo 'Test stage'
      }
    }
    stage('Deliver') {
      steps {
        echo 'Deliver stage'
      }
    }
    stage('Cleanup') {
      steps {
        echo 'Cleanup stage'
      }
    }
  }
  environment {
    CI = 'True'
  }
}