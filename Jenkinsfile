pipeline {
  agent any
  stages {
    stage('Sonarqube') {
      environment {
        scannerHome = 'sonar_scanner'
      }
      steps {
        withSonarQubeEnv('SonarQube') {
          sh "${scannerHome}/bin/sonar-scanner"
        }

        timeout(time: 10, unit: 'MINUTES') {
          waitForQualityGate true
        }

      }
    }
  }
}