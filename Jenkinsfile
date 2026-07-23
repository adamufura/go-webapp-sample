pipeline{
  agent any
  tools {
    go 'go1.26.5'
  }

  environment {
    GO111MODULE = 'on'
    CGO_ENABLED = '1'
  }

  stages{
    stage('Test') {
      steps {   
        git 'https://github.com/adamufura/go-webapp-sample.git'
        sh 'go test ./...'
      }
    }
  }
}