pipeline {
  agent any
  stages {
    stage('Verify browsers are installed') {
      steps {
        sh 'firefox --version'
      }
    }
    stage('Run Tests') {
      steps {
        sh './mvnw clean test'
      }
    }
  }
}