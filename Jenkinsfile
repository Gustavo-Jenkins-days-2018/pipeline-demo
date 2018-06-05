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
  parameters {
      string(name: 'Name', defaultValue: 'whoever you are', 
	     description: 'Who should I say hi to?')
   }
  stages {
    stage('say Hello') {
      steps {
        echo "Env value: Hello ${MY_NAME}!"
	echo "HParam value: ello ${params.Name}!"
        echo "${TEST_USER_USR}"
        echo "${TEST_USER_PSW}"
        sh 'java -version'
      }
    }
  }
}
