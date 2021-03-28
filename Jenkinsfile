pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        powershell 'build.gradle'
        powershell 'gradle doc'
      }
    }

    stage('Mail Notification') {
      steps {
        mail(subject: 'Succes', body: 'build avec succes', cc: 'hc_serbouh@esi.dz', bcc: 'hc_serbouh@esi.dz')
      }
    }

  }
}