pipeline {
  agent any
  stages {
    stage('Intialize') {
      steps {
        sh 'mvn clean'
      }
    }
    stage('Build') {
      steps {
        sh 'mvn install package'
      }
    }
  }
}