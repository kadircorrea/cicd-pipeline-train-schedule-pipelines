pipeline {
  agent any
  stages{
    stage ('build'){
      steps{
        echo "Building"
        sh './gradlew build --no-daemon'
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}
