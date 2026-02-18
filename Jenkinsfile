pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }
        stage('Build') {
            steps {
                sh 'echo Building the project...'
            }
        }
        stage('Sonar Scan') {
            steps {
                sh 'echo Performing SonarQube analysis...'
            }
        }
        stage('Download from Artifactory') {
            steps {
                sh 'echo Downloading artifacts from Artifactory...'
            }
        }
    }
}