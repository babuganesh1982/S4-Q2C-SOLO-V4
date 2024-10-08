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
    stage('explicityly run get-usebruno-user-information') {
      steps {
        dir('TestJenkinsBru') {
          sh '''
            bru run get-usebruno-user-information.bru
          '''
        }
      }
    }
  }
}