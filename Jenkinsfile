pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Hello, Bees!!!!'
        writeFile file: "application.sh", text: "echo Built ${BUILD_ID} of ${JOB_NAME}"
        archiveArtifacts artifacts: '*.sh', fingerprint: true
      }
    }
  }
}
