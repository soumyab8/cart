pipeline {
    agent any
    stages {
        stage('Lint checks') {
                steps {
                    sh "echo installing jslint"
                    sh "npm install jslint"
                    sh "ls -ltr node_modules/jslint/bin"
                    sh "~/node_modules/jslint/bin/jslint.js server.js || true"
                    sh "echo lint checks completed"
                }
        }
    }
}