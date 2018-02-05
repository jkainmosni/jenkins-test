pipeline {
  agent any
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
        stage('this job wont work') {
          steps {
            sh 'zsexrdctfvgbhnjmk'
          }
        }
      }
    }
  }
}