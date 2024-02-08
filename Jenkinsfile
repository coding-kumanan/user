@Library('roboshop-shared-library@main') _
pipeline {
    agent any 
    stages {
        stage('Lint Checks') {
            steps {
                script {
                    sample.info("learndevopswithcloud")
                }
                sh "echo Starting lintchecks"
                sh "echo Installing JSlist"
                sh "npm i jslint"
                sh "node_modules/jslint/bin/jslint.js server.js || true"
                sh "echo lintchecks completed sucessfully"
            }
        }
        stage('Generating the artifacts..') {
            steps {
                //sh "npm install"
                sh "echo npm"
            }
        }
    }
}