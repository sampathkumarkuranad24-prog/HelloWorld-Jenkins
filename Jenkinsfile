pipeline {
    agent any

    stages {

        stage('Build') {
            steps {
                bat 'javac Hello.java'
            }
        }

        stage('Test') {
            steps {
                bat 'java Hello'
            }
        }

        stage('Archive') {
            steps {
                archiveArtifacts artifacts: 'Hello.class', fingerprint: true
            }
        }
    }
}
