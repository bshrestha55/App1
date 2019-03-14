pipeline {
    agent any
    stages {

        stage('Build') {
            steps {
                sh 'mvn clean'
                sh 'mvn compile'
            }

        }

        stage('Deploy') {
            steps {
                sh 'echo "Deploying files"'
            }
        }

        stage('Unit Test') {
            steps {
                sh 'echo "Running Unit Test"'
            }
        }
    }
}
