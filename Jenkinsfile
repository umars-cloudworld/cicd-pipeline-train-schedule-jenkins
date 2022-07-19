pipeline {
  agent any
  stages {
    stage ('Build') {
      steps {
        echo "Build the project"
        sh './gradlaw build --no-daemon'
      }
    stage ('Artifactes') {
      steps {
        echo "Building the project artifacts"
        archieveArtifcates artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}
