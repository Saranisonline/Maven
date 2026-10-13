pipeline {
    agent any

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

    post {
        success {
            echo 'BUILD SUCCESS!'
        }

        failure {
            echo 'BUILD FAILED!'
        }
    }
}
