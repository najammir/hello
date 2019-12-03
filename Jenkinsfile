pipeline {
  agent any
  stages {
    stage('sonarqube') {
      steps {
        sh '''cd /var/lib/jenkins/plugins/sonar/META-INF/maven/org.jenkins-ci.plugins/sonar
mvn sonar:sonar -Dsonar.host.url=http://172.30.219.110:9000 -Dlicense.skip=true'''
      }
    }
  }
}