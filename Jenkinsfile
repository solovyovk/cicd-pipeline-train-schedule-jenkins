pipeline {
  agent any
  stages {
    stage ('Build') {
      steps {
        echo 'Build an train-schedule app'
        sh './gradlew build --no-daemon'
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}
