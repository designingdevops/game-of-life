pipeline {
  agent {
    docker {
      label "docker"
      image" maven-jdk-8"
    }
  }
  stages {
    stage('build') {
      steps {
        sh "mvn clean package"
      }
    }
  }
}
