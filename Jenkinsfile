pipeline {
  agent any
  stages {
    stage('Checkout') {
      steps {
        git(url: 'https://github.com/Omkar-Shetkar/spring-test-containers-jenkins.git', branch: 'main', credentialsId: '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')
      }
    }

    stage('tests') {
      steps {
        sh './mvnw clean test'
      }
    }

  }
}