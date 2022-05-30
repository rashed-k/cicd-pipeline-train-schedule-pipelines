pipeline {
  agent any
  stages {
    steps ('Build') {
      steps {
        echo 'Running Building automation'
        sh './gradlew build --no-daemon'
        archiveArtifcats artifacts: 'dist/trainSchedule.zip'
      }   
    }
  }
}
