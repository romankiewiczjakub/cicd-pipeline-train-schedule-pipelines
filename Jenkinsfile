pipeline {
  agent any
  stages {
    stage ('Build') {
      steps {
        echo 'Running build atuomation'
        sh "./gradlew build --no-daemon"
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}
