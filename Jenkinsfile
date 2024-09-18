pipeline {
  agent any
  stages {
    stage('Build') {
      step {
        echo 'Running a building operation'
        sh './gradlew build --no-demon'
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}
