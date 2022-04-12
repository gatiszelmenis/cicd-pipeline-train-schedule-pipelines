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
    stage ('test') {
      steps {
        echo 'Running a build test now ...'
        sh 'uptime'
      }
    }
    stage ('Final') {
      steps {
        echo 'Running a Final touch test now ...'
        sh 'uname -a'
      }
    }
  }
}
