pipeline {
  agent any
  stages {
    stage('verify installation') {
      steps {
       powershell 'bru --version'
      }
    }
    stage('run all files in the collection') {
      steps {
        dir('TestJenkinsBru') {
         powershell 'bru run --env CC3-702'
        }
      }
    }
  }
}
