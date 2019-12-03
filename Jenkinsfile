pipeline {
  agent any
  stages {
    stage('') {
      steps {
        sh 'mvn sonar:sonar -Dsonar.host.url=http://172.30.219.110:9000 -Dlicense.skip=true'
      }
    }
  }
}