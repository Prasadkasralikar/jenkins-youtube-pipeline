pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh '''pwd
date'''
      }
    }

    stage('test-stage') {
      parallel {
        stage('test-stage') {
          steps {
            echo 'test step'
          }
        }

        stage('test par') {
          steps {
            echo 'test [par]'
          }
        }

      }
    }

    stage('deploy') {
      steps {
        echo 'deploy'
        sleep 3
      }
    }

  }
}