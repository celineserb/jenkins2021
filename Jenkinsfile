pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        withGradle() {
          powershell 'gradle build'
        }

      }
    }

  }
}