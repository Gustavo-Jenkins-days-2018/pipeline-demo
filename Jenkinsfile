pipeline {
  agent {
    node {
      label 'jdk8'
    }

  }
  stages {
    stage('say Hello') {
      steps {
        echo 'Hello World 2'
        sh 'java -version'
      }
    }
  }
}
