pipeline {
    agent{
        docker {
            image "node:20-alpine"
        }
    }
    stages{
        stage("Build") {
            steps {
                sh "npm install"
            }
        }
    }
}