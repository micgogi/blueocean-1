pipeline {
  agent {
    docker {
      image 'maven:3-alpine'
      args '-v /opt/m2:/root/.m2'
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