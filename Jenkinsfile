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
    stage('build') {
      steps {
        bat 'mvn clean install'
      }
    }
    stage('Junit Test') {
      steps {
        bat 'mvn test'
      }
    }
    stage('sonar') {
      steps {
        bat 'mvn sonar:sonar'
      }
    }
  }
}