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
              sh 'cd app/demoapp && mvn clean compile'
          }
      }

    stage('Test') {
        steps {
            sh 'cd app/demoapp && mvn test'
         }
     }

    stage('Package') {
       steps {
          sh 'cd app/demoapp && mvn package'
         }
       }
    }
}
