pipeline {
  agent any
  stages {
    stage('Checkout') {
      steps {
        git(url: 'https://github.com/Omkar-Shetkar/spring-test-containers-jenkins', branch: 'main')
      }
    }

    stage('tests') {
      steps {
        sh './mvnw clean test'
      }
    }

  }
}