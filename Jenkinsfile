pipeline {
  agent any
  stages {
    stage('checkout') {
      steps {
        git(url: 'https://github.com/krishna7362/os-sample-java-web.git', branch: 'master')
      }
    }
    stage('build') {
      steps {
        bat 'mvn package'
      }
    }
  }
}