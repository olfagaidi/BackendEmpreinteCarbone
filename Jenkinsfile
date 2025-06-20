pipeline {
  agent any
  stages {
    stage('Checkout') {
      steps {
        git(url: 'https://github.com/olfagaidi/BackendEmpreinteCarbone.git', branch: 'main', credentialsId: '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', poll: true, changelog: true)
      }
    }

    stage('Build Docker Image') {
      steps {
        sh 'docker build -t empreinte-backend -f Dockerfile.backend .'
      }
    }

    stage('Run Container') {
      steps {
        sh 'docker run -d -p 5000:80 empreinte-backend'
      }
    }

  }
}