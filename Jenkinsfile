pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        git(url: 'git@github.com:Czhengxi/FirstProject.git', branch: 'dev')
        bat 'mvn clean package'
      }
    }

    stage('test') {
      steps {
        bat 'mvn clean test'
      }
    }

  }
}