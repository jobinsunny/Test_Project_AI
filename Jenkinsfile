pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/your-repo/your-project.git' // Update with your repo URL
            }
        }
        stage('Maven Build') {
            steps {
                sh 'mvn clean install'
            }
        }
        stage('Sonar Scanning') {
            steps {
                sh 'mvn sonar:sonar'
            }
        }
        stage('Artifactory Download') {
            steps {
                sh 'curl -u user:password "https://your.artifactory.server/artifactory/repo/path/to/artifact" -O'
            }
        }
    }
}