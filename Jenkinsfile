pipeline {
  agent {
    docker {
      args '-v /root/.m2:/root/.m2'
      image 'maven:3.8.1-jdk-8'
    }

  }
  stages {
    stage('Build') {
      steps {
        sh 'sh \'mvn -B -DskipTests clean package\''
      }
    }

  }
}