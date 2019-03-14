pipeline {
    agent any
    stages {

        stage('Build') {
            steps {
                withMaven(maven: 'maven_3_6_0'){
                  sh 'mvn clean'
                  sh 'mvn compile'
                }
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
