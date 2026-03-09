pipeline {
    agent any
    stages {
        stage('Create HTML') {
            steps {
                
            }
        }
        stage('Publish') {
            steps {
                publishHTML([
                    allowMissing: false,
                    alwaysLinkToLastBuild: true,
                    keepAll: true,
                    reportDir: 'reports',
                    reportFiles: 'index.html',
                    reportName: 'Simple Report'
                ])
            }
        }
    }
}
