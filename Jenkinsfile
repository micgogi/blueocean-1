pipeline {
  agent {
    docker {
      image 'maven:3-alpine'
      args '-v /root/.m2:/root/.m2'
    }

  }
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