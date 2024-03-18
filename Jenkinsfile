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
               // bat """mvn clean install"""
                echo 'Hello Pipeline' 
            }
        }
    }
}
