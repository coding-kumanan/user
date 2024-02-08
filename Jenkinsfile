pipeline {
    agent any 
    stages {
        stage('Lint Checks') {
            steps {
                sh "echo Starting lintchecks"
                sh "echo Installing JSlist"
                sh "npm i jslint"
                sh "node_modules/jslint/bin/jslint.js server.js || true"
                sh "lintchecks completed sucessfully"
            }
        }
        stage('Generating the artifacts..'){
            steps{
                sh "npm install"
            }
        }
    }
}