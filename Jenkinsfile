pipeline {
  agent any
  tools{
      maven "maven-3.6.3"
  }
  stages {
    stage('Verify browsers are installed') {
      steps {
        sh 'firefox --version'
      }
    }
    stage('Run Tests') {
      steps {
        sh 'mvn clean test'
      }
    }
  }
}