pipeline {
  agent any

  stages {
    stage('Remote Command') {
      steps {
        sshagent(['slave1-cred'])  {
          sh 'ssh  -o StrictHostKeyChecking=no  slave1-cred@13.232.44.132 "sudo su -"'
        }
      }
    }
  }
}

