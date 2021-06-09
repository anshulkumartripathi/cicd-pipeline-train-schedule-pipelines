pipeline {
  agent any
  stages {
    stage ('Build') {
      steps {
        echo 'Building the project'
        sh './gradlew build --no-daemon'
        archiveArtifacts artifact: 'dist/trainSchedule.zip'
      }
    }
  }
}
