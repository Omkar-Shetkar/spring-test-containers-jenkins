pipeline {
  agent any
  stages {
    stage('Checkout') {
      steps {
        git(url: 'git@github.com:Omkar-Shetkar/spring-test-containers-jenkins.git', branch: 'main')
      }
    }

    stage('tests') {
      steps {
        sh './mvnw clean test'
      }
    }

  }
}