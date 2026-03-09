pipeline {
    agent any

    stages {
        stage('Fecth file') {
            steps {
                git 'https://github.com/itsroshravi/javarep.git'
            }
        }
        stage('Building') {
            steps {
                echo 'Building Project .....'
                bat 'javac Hello.java'
            }
        }
        stage('Executing') {
            steps {
                echo 'Executing Program'
                bat 'java Hello'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying .....'
            }
        }
    }
    post{
        success{ 
            echo 'Pipeline Executed Successfully'
        }
        failure{
            echo 'Pipeline Failed'
        }
    }
}
