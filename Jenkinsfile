pipeline {
  agent any

  stages {
    stage('Remote Command') {
      steps {
        sshagent(['slave1-cred'])  {
          sh 'ssh -i ~/.ssh/id_rsa slave1-cred@13.232.44.132 "sudo su -"'
        }
      }
    }
  }
}

