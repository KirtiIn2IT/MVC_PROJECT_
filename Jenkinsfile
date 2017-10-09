pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        bat 'echo Build'
      }
    }
    stage('Test') {
      steps {
        parallel(
          "Test": {
            bat 'echo Test'
            
          },
          "More Test": {
            bat 'echo MoreTest'
            
          }
        )
      }
    }
    stage('Deploy') {
      steps {
        bat 'echo Deploy'
      }
    }
  }
}