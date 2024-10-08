pipeline {
  agent any
  stages {
    stage('verify installation') {
      steps {
        sh 'bru --version'
      }
    }
    stage('run all files in the collection') {
      steps {
        dir('TestJenkinsBru') {
          sh 'bru run'
        }
      }
    }
  }
}
