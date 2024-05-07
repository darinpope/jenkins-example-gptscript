pipeline {
  agent { label 'gptscript' }
  environment {
    OPENAI_API_KEY=credentials('openai-api-key')
  }
  stages {
    stage('verify installation') {
      steps {
        sh 'gptscript -v'
      }
    }
    stage('run hello world') {
      steps {
        sh 'gptscript https://get.gptscript.ai/echo.gpt --input "Hello, World!"'
      }
    }
    stage('run bob') {
      steps {
        sh 'gptscript bob.gpt'
      }
    }
  }
}