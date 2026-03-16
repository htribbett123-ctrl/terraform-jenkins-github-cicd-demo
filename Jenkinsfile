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
                dir('app/demoapp') {
                    sh 'mvn clean compile'
                }
            }
        }

        stage('Test') {
            steps {
                dir('app/demoapp') {
                    sh 'mvn test'
                }
            }
        }

        stage('Package') {
            steps {
                dir('app/demoapp') {
                    sh 'mvn package'
                }
            }
        }
    }
}
