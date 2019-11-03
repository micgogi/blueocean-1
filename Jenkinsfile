pipeline {
  agent {
    docker {
      args '-v /opt/m2:/root/.m2'
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