pipeline {
  agent any
  stages {
    stage('compile') {
      steps {
        sh 'java -version'
      }
    }

    stage('Test') {
      steps {
        sh 'mvn test'
      }
    }

    stage('Deploy') {
      steps {
        sh 'mvn package -DskipTests'
      }
    }

  }
}