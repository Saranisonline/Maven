pipeline {
    agent any

    tools {
        jdk 'jdk-21.0.12'
        maven 'Maven-3'
    }

    stages {

        stage('Check Java and Maven') {
            steps {
                bat 'java -version'
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
            echo 'Maven build completed successfully!'
        }

        failure {
            echo 'Maven build failed!'
        }
    }
}
