pipeline {
    agent any

    tools {
        maven 'Maven-3'
    }

    stages {

        stage('Check Java') {
            steps {
                bat 'java -version'
            }
        }

        stage('Check Maven') {
            steps {
                bat 'mvn -version'
            }
        }

        stage('Build') {
            steps {
                bat 'mvn clean package'
            }
        }
    }
}
