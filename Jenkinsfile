pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Starting'
        sh 'npm install'
      }
    }

    stage('Test') {
      steps {
        sh 'npm run test'
      }
    }

    stage('Package') {
      steps {
        sh 'npm run package'
      }
    }

    stage('Post Build Actions') {
      steps {
        archiveArtifacts(artifacts: '*.zip', onlyIfSuccessful: true)
      }
    }

  }
  environment {
    Foo = 'Bar'
  }
}