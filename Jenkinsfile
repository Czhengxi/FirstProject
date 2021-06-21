pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        git(url: 'https://gitee.com/chen-zhengxi/jenkins-study.git', branch: 'master')
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