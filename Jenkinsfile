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
        stage('Build') {
            steps {
                nexusArtifactUploader artifacts: [[artifactId: '', classifier: '', file: 'nexus', type: 'txt']], credentialsId: 'c1e176e2-d3ac-4225-937e-42c0457ed05f', groupId: '', nexusUrl: 'localhost:8081', nexusVersion: 'nexus3', protocol: 'http', repository: 'Myfile', version: ''
               }
    }

    }
}
