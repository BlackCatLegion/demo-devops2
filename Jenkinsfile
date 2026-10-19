pipeline {
    agent any
    stages {
        stage('Clone Code') {
            steps { git branch: 'main', url: 'https://github.com/blackcatlegion/devops-practice.git' }
        }
        stage('Build') {
            steps { sh 'mvn clean compile' }
        }
        stage('Test') {
            steps { sh 'mvn test' }
        }
        stage('Package') {
            steps { sh 'mvn package' }
        }
        stage('Deploy') {
            steps { echo 'Deploy placeholder' }
        }
    }
}
