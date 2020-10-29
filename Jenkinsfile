pipeline {
  agent any
  stages {
    stage('checkout') {
      steps {
        git(url: 'https://github.com/ukkiran/maven-project-1.git', branch: 'master', credentialsId: 'github')
      }
    }

    stage('build') {
      steps {
        build 'mvn clean package'
      }
    }

  }
}