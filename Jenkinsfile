pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'build.gradle'
      }
    }

    stage('Mail Notification') {
      steps {
        mail(subject: 'Succes/Echec', body: 'build avec succés', cc: 'hc_serbouh@esi.dz')
      }
    }

  }
}