pipeline {
  agent {
    dockerfile {
      filename 'Dockerfile'
    }
    
  }
  stages {
    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            sh 'sudo docker build --tag="ubiworx-test-replay" .'
          }
        }
        stage('Run') {
          steps {
            sh 'sudo docker run -d ubiworx-test-replay'
          }
        }
      }
    }
  }
}