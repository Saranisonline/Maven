pipeline {
    agent any

    tools {
        maven 'Maven-3'
    }

    stages {

        stage('Java Check') {
            steps {
                bat 'java -version'
            }
        }

        stage('Maven Check') {
            steps {
                bat 'mvn -version'
            }
        }

        stage('Maven Build') {
            steps {
                bat 'mvn clean package'
            }
        }
    }
}
