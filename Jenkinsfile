pipeline {
    agent {
        docker {
            image "node:20-alpine"
        }
    }
    stages {
        stage("Build") {
            steps {
                sh "chmod +x ./scripts/dropdb.sh"
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