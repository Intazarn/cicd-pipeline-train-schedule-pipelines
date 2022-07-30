pipeline {
  agent any
  stages {
    stage ('Build') {
      steps {
         echo 'Running Build Automation'
         sh './gradlew build --no-daemon'
         sh './gradlew npm_start'
         archieveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
  
}
