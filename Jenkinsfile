pipeline {
  agent {
    docker {
      image 'maven'
    }
    
  }
  stages {
    stage('Build') {
      steps {
        sh 'mvn package'
      }
    }
    stage('Verify') {
      steps {
        parallel(
          "Verify": {
            sh 'mvn verify'
            
          },
          "Parallel": {
            sh 'sleep 30'
            
          }
        )
      }
    }
  }
}
