pipeline {
    agent any

    stages {
        stage('Checkout'){
            steps{
                git 'https://github.com/itsroshravi/javarep'
            }
        }
        stage('Build') {
            steps {
                echo 'Compiling Java program...'
                bat 'javac Hello.java'
            }
        }

        stage('Execute') {
            steps {
                echo 'Running Java program...'
                bat 'java Hello'
            }
        }
    }

    post {
        success {
            echo 'Pipeline completed successfully!'
        }
        failure {
            echo 'Pipeline failed!'
        }
    }
}
