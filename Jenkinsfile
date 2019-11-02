pipeline {
  agent {
    docker {
      image 'maven:3.5-jdk-8-slim'
    }

  }
  stages {
    stage('clean') {
      steps {
        sh 'mvn clean'
      }
    }
    stage('build') {
      steps {
        sh 'mvn install package'
      }
    }
  }
}