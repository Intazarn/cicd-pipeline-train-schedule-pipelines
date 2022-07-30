pipeline {
  agent any
  stages {
    stage ('Build') {
      steps {
         echo 'Running Build Automation'
         sh './gradlew build --no-daemon'
         archieveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
  
}
