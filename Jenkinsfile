pipeline {
  agent any
  stages {
    stage('checkout') {
      parallel {
        stage('checkout') {
          steps {
            echo 'hello'
          }
        }

        stage('build') {
          steps {
            sh 'mvn clean install'
          }
        }

      }
    }

  }
}
