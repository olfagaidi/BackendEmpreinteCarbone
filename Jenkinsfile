pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git credentialsId: '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', url: 'https://github.com/olfagaidi/BackendEmpreinteCarbone.git', branch: 'main'
            }
        }

        stage('Build Docker Image') {
            steps {
                script {
                    docker.build("mon-pfe-backend", "-f Dockerfile.backend .")
                }
            }
        }

        stage('Run Container') {
            steps {
                script {
                    docker.image("mon-pfe-backend").run("-d -p 8080:80")
                }
            }
        }
    }
}
