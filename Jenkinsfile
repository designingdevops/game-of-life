pipeline {
  agent {
    docker {
      image "maven"
      label "docker"
    }
  }
  stages {
    stage('build') {
      steps {
        sh "mvn clean package site"
      }
    }
  }
}
