pipeline {
  agent {
    docker {
      label "docker"
      image" maven"
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
