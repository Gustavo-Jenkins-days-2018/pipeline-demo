pipeline {
  agent {
    node {
      label 'jdk8'
    }

  }
  environment {
      MY_NAME = 'Gustavo'
   }
  stages {
    stage('say Hello') {
      steps {
        echo "Hello ${MY_NAME}!"
        sh 'java -version'
      }
    }
  }
}
