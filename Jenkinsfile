



pipeline{
      agent any 

stages{

           stage('Remote Access') {

                      agent any


                steps {
                    sshagent(['slave-node-2']) {
            sh 'ssh -o StrictHostKeyChecking=no ec2-user@3.108.65.248  sudo su -'
                  }
                }
            }

}

}
