pipeline {
  agent any
  stages {
    stage('Build') {
      agent {
        docker {
          image 'maven:3.5-jdk-8-slim'
        }

      }
      steps {
        sh '''

echo "Hello World"




mvn clean
mvn install package'''
      }
    }
  }
}