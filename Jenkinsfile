pipeline {
  agent any

  stages {
    stage('Checkout') {
      steps {
        git 'https://github.com/olfagaidi/BackendEmpreinteCarbone.git'
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
