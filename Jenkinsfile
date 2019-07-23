pipeline {
  agent any
  stages {
    stage('checkout') {
      steps {
        git 'https://github.com/krishna7362/os-sample-java-web.git'
      }
    }
    stage('compile') {
      steps {
        bat 'mvn compile'
      }
    }
  }
}