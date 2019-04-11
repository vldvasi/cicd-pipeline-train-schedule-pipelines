pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Running the build automation'
        sh './gradlew build --no-daemon'
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    
    }
    stage('Test') {
      steps {
        echo 'Running the testing'
      }
    
    }
  }

}
