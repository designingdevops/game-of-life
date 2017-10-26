pipeline {
  agent {
    docker {
      image 'maven'
    }
    
  }
  stages {
    stage('Compile') {
      steps {
        sh 'mvn package'
      }
    }
    stage('Test') {
      steps {
        sh 'mvn verify'
      }
    }
  }
}