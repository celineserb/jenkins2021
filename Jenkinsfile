pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        powershell 'build.gradle'
        powershell 'gradle doc'
        junit 'Results'
      }
    }

  }
}