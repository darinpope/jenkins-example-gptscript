pipeline {
  agent { label 'gptscript' }
  stages {
    stage('verify installation') {
      steps {
        sh 'gptscript -v'
      }
    }
  }
}