pipeline {
  agent any
  stages {
    stage('test1') {
      steps {
        timestamps() {
          bat(script: 'hostname', returnStdout: true)
        }
        
      }
    }
  }
}