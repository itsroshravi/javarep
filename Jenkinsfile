pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/itsroshravi/javarep.git'
            }
        }
        stage('Publish') {
            steps {
                publishHTML([
                    
                    allowMissing: true,
                    alwaysLinkToLastBuild: false,
                    keepAll: false,
                    reportDir: '.',
                    reportFiles: 'servehtml.html',
                    reportName: 'MY HTML PAGE'
                    
                ])
            }
        }
    }
}
