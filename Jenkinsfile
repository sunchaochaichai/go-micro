pipeline {
  agent any
  stages {
    stage('test') {
      steps {
        sh 'echo "test"'
      }
    }
    stage('build') {
      parallel {
        stage('build') {
          steps {
            sh 'echo "build"'
          }
        }
        stage('build1') {
          steps {
            sh 'echo "build1"'
          }
        }
      }
    }
    stage('deploy') {
      steps {
        sh 'echo "deploy"'
      }
    }
  }
}