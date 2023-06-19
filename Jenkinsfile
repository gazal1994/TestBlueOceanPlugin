pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'build completed'
      }
    }

    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            echo 'Runnig Test2'
          }
        }

        stage('Test1') {
          steps {
            echo 'Running Test1'
          }
        }

      }
    }

    stage('deploy') {
      steps {
        echo 'deply comleted'
      }
    }

  }
}