pipeline {
  agent any
  stages {
    stage('verify installation') {
      steps {
        bat 'bru --version'
      }
    }
    stage('run all files in the collection') {
      steps {
        dir('TestJenkinsBru') {
          bat 'bru run --env CC3-702'
        }
      }
    }
  }
}
