pipeline {
    agent {
        node {
            label 'node'
        }
    }
    stages {
        stage('Checkout code'){
            steps {
                 checkout scm
            }
       }
        stage('Build') {
            steps {
                echo 'Building..'
                sh 'ls -la'
                sh './spring-petclinic/mvnw'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
