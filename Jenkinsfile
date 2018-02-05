pipeline {
  agent {
    node {
      label 'some-label'
    }
    
  }
  stages {
    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            sh 'echo "hello"'
          }
        }
        stage('Run') {
          steps {
            sh 'date'
          }
        }
      }
    }
  }
}