pipeline {
  agent any
  stages {
    stage('verify installation') {
      steps {
        'bru --version'
      }
    }
    stage('run all files in the collection') {
      steps {
        dir('TestJenkinsBru') {
          'bru run --env CC3-702'
        }
      }
    }
  }
}
