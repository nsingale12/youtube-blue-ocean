pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh '''pwd
ls -ltr'''
      }
    }

    stage('test') {
      parallel {
        stage('test') {
          steps {
            echo 'tst step'
          }
        }

        stage('') {
          steps {
            echo 'parallel'
          }
        }

      }
    }

    stage('') {
      steps {
        sleep 30
      }
    }

  }
}