pipeline {
  agent none
  stages {
    stage('test') {
      steps {
        sh 'echo hi'
      }
    }
    stage('build') {
      steps {
        sh 'mvn -Dtest=Account clean test -Dcucumber.options="--tags @AIL"'
      }
    }
  }
}