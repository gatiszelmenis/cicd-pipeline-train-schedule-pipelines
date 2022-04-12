pipeline {
  agent any
  stages {
    stage ('build') {
      steps {
        echo 'Running a build now ...'
        sh './gradlew build --no-daemon'
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}
