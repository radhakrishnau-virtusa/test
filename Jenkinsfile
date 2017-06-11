pipeline {
  agent {
    dockerfile {
      filename 'hhhh'
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
            
            echo 'kjv'
            
          }
        )
      }
    }
    stage('thhhh') {
      steps {
        parallel(
          "thhhh": {
            readTrusted 'gg'
            
          },
          "": {
            echo 'hhh'
            
          }
        )
      }
    }
  }
}