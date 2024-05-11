pipeline {
    agent {
        docker {
            image "node:20-alpine"
        }
    }
    stages {
        stage("Build") {
            steps {
                sh "npm install"
            }
        }
        stage("Test") {
            steps{
                sh "npm run test:ci"
            }
        }
    }
}