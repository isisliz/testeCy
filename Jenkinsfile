pipeline {
    agent any

    tools { nodejs 'NodeJS Plugin' }

    stages {
        stage('Install dependencies') {
            steps {
                sh 'npm install'
            }
        }
        stage('Running production backtests') {
            steps {
                sh 'npm run prod:regress'
            }
        }
    }
}
