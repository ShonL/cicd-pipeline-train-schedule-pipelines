pipeline {
  agent any
  stages {
    stage ('Build') {
      steps {
        eacho 'Running build automation (shon)...'
        sh './gradlew build --no-deamon'
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}
