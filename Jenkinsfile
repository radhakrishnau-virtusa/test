pipeline {
  agent {
    node {
      label 't'
    }
    
  }
  stages {
    stage('Build') {
      steps {
        parallel(
          "test": {
            timestamps() {
              bat(script: 'hostname', returnStdout: true)
            }
            
            
          },
          "test24": {
            echo 'fg'
            
          }
        )
      }
    }
    stage('Test') {
      steps {
        bat(script: 'test', returnStdout: true)
      }
    }
  }
}