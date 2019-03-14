pipeline {
    agent any
    stages {
        stage('Compile') {
            steps {
                withMaven(maven: 'maven_3_6_0'){
                  sh 'mvn clean compile'
                }
            }

        }

        stage('Unit Test') {
            steps {
                withMaven(maven: 'maven_3_6_0'){
                  sh 'mvn test'
                }
            }
        }

        stage('Package') {
            steps {
              withMaven(maven: 'maven_3_6_0'){
                sh 'mvn package'
              }
            }
        }

        stage('Deploy') {
            steps {
                sh 'echo "Deploying files"'
            }
        }
    }
}
