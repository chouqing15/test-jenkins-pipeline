pipeline {
    agent { docker 'node:16.14.0' }

    environment {
        NPM_CONFIG_CACHE = "${WORKSPACE}/.npm"
    }
    
    stages {
        stage('build') {
            steps {
                sh 'npm install'
                sh 'npm run build'
            }
        }
    }
}