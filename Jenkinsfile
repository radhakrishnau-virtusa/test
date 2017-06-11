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
        parallel(
          "Test": {
            bat(script: 'test', returnStdout: true)
            
          },
          "load": {
            script {
              echo test
            }
            
            
          }
        )
      }
    }
  }
}