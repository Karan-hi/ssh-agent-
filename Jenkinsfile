pipeline {
  agent any

  stages {
    stage('Remote Command') {
      steps {
        sshagent([credentialsId: 'slave-cred']) {
          sh 'ssh -i ~/.ssh/id_rsa slave2@65.1.92.138 "sudo su -"'
        }
      }
    }
  }
}

