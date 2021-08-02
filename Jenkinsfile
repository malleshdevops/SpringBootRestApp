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

        stage('Maven3') {
          agent any
          environment {
            maven = 'Maven3'
          }
          steps {
            sh 'mvn clean install'
          }
        }

      }
    }

  }
}