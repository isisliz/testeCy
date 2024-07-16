pipeline {
    agent any

    tools { nodejs 'NodeJS Plugin' }

    stages {
        stage('Install dependencies') {
            steps {
                bat 'npm install'
            }
        }
        stage('Running production backtests') {
            steps {
                bat 'npm run cypress:run'
            }
        }
    }
}
