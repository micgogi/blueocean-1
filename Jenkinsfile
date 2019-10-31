pipeline {
  agent {
    docker {
      args '''args  "--entrypoint=\'\' "
-v /root/.m2:/root/.m2'''
      image 'maven:3-jdk-8'
    }

  }
  stages {
    stage('Intialize') {
      steps {
        sh '''echo PATH= ${PATH}
echo M2_HOME = ${M2_HOME}
mvn clean'''
      }
    }
  }
}