pipeline {
  agent any
  stages {
    stage ('Build') {
      steps {
        echo 'Running build automation (shon)...'
        sh './gradlew build --no-deamon'
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}
