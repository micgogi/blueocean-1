pipeline {
  agent {
    docker {
      image 'maven:3.5-jdk-8-slim'
    }
  }
  stages {
    stage('Build') {
      steps {
        sh 'echo "Hello World"'
      }
    }
  }
}
