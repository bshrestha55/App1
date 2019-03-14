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
                sh 'whoami'
                sh 'ls /Users/shrbi001/Documents/jar'
                sh 'touch /Users/shrbi001/Documents/jar/apple.txt'
                sh 'cp target/app1-0.0.1-SNAPSHOT.jar /Users/shrbi001/Documents/jar/app1.jar'
              }
            }
        }

        stage('Deploy') {
            steps {
                sh 'java -jar /Users/shrbi001/Documents/app1.jar'
            }
        }
    }
}
