pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/htribbett123-ctrl/terraform-jenkins-github-cicd-demo.git'
            }
        }

        stage('Build') {
            steps {
                bat 'echo Building application'
            }
        }

        stage('Test') {
            steps {
                bat 'echo Running tests'
            }
        }

        stage('Deploy') {
            steps {
                bat 'echo Deploying'
            }
        }

    }
}

