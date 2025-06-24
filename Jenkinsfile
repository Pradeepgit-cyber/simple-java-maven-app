pipeline {
    agent any
    tools {
        maven 'HomebrewMaven'
    }
    stages {
        stage('Build') {
            steps {
                sh 'echo "Building the Maven Project..."'
                sh 'mvn clean package'
            }
        }
        stage('Test') {
            steps {
                sh 'echo "Running Tests..."'
                sh 'mvn test'
            }
        }
    }
}
