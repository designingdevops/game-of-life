pipeline {
  agent {
    docker {
      label "docker"
      image" maven:latest"
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
