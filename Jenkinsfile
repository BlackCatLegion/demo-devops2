pipeline {
    agent any
    stages {
        steps { git branch: 'main', url: 'https://github.com/BlackCatLegion/demo-devops2.git' }
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
