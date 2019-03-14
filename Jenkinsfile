pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                sh 'echo "Checking out files"'
            }
        }

        stage('Build') {
            steps {
                sh 'echo "Building files"'
            }
        }

        stage('Deploy') {
            steps {
                sh 'echo "Deploying files"'
            }
        }

        stage('Unit Test') {
            steps {
                sh 'Running Unit Test'
            }
        }
    }
}
