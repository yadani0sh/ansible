pipeline {
  agent any
  stages {
    stage('biuld') {
      steps {
        sh 'mvn clean'
      }
    }

    stage('test') {
      steps {
        sh 'mvn test'
      }
    }

    stage('deploy') {
      steps {
        sh 'mvn package'
      }
    }

  }
}