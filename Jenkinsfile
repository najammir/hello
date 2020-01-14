pipeline {
  agent any
  stages {
    stage('deploy') {
      steps {
        sh '''cd /var/lib/jenkins/workspace/hello_master/
sudo chmod 777 bash.sh
./bash.sh'''
      }
    }
  }
}