pipeline {
  agent {
    node {
      label 'jdk8'
    }

  }
  environment {
      MY_NAME = 'Gustavo'
      TEST_USER = credentials('test-user')
   }
  stages {
    stage('say Hello') {
      steps {
        echo "Hello ${MY_NAME}!"
        echo "${TEST_USER_USR}"
        echo "${TEST_USER_PSW}"
        sh 'java -version'
      }
    }
  }
}
