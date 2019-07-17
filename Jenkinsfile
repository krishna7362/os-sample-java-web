pipeline {
  agent any
  stages {
    stage('checkout') {
      steps {
        git(url: 'https://github.com/krishna7362/os-sample-java-web.git', branch: 'master')
      }
    }
    stage('build') {
      parallel {
        stage('build') {
          steps {
            bat 'mvn compile'
          }
        }
        stage('sonar') {
          steps {
            bat 'mvn sonar:sonar'
          }
        }
      }
    }
  }
}