pipeline {
  agent {
    docker {
      image 'maven:3.5-jdk-8-slim'
    }

  }
  stages {
    stage('initial') {
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