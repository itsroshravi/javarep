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
                    
                    reportDir: 'reports',
                    reportFiles: 'servehtml.html',
                    reportName: 'MY HTML PAGE'
                ])
            }
        }
    }
}
