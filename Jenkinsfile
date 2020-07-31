pipeline {
  agent any
  stages {
    stage('f') {
      steps {
        archiveArtifacts(artifacts: '1111', allowEmptyArchive: true, caseSensitive: true, defaultExcludes: true, excludes: '2222', fingerprint: true, onlyIfSuccessful: true)
      }
    }

  }
}