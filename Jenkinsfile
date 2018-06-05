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
      string(name: 'Name:', defaultValue: 'Enter your first name', 
	     description: 'Who should I say hi to?')
   }
  stages {
    stage('say Hello') {
      steps {
        echo "Env value: Hello ${MY_NAME}!"
	echo
	echo "Param value: Hello ${params.Name}!"
	echo
        echo "${TEST_USER_USR}"
        echo "${TEST_USER_PSW}"
        sh 'java -version'
      }
    }
  }
}
