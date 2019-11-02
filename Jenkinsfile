pipeline {
  agent {
    docker {
      image ' maven:3.5-jdk-8-slim '
    }

  }
  stages {
    stage('clean') {
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