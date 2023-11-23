pipeline {
    agent any
    stages {
        stage('Test') {
            steps {
                sh 'node --version'
            }
        }
        stage('Build') {
            steps {
                sh '/usr/bin/docker pull gradle:8.2.0-jdk17-alpine'
                sh '/usr/bin/docker inspect -f . gradle:8.2.0-jdk17-alpine'
                // Other commands related to Docker using the full path
            }
        }
    }
}
