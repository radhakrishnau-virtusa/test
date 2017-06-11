pipeline {
  agent any
  stages {
    stage('test1') {
      steps {
        load 'test2.groovy'
        timestamps() {
          bat(script: 'hostname', returnStdout: true)
        }
        
      }
    }
  }
}