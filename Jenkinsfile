pipeline {
    agent any

    stages {

        stage('Java Check') {
            steps {
                bat 'java -version'
            }
        }

        stage('Maven Check') {
            steps {
                bat '"C:\\Users\\STUDENT\\Downloads\\apache-maven-3.10.0-bin\\apache-maven-3.10.0\\bin\\mvn.cmd" -version'
            }
        }

        stage('Maven Build') {
            steps {
                bat '"C:\\Users\\STUDENT\\Downloads\\apache-maven-3.10.0-bin\\apache-maven-3.10.0\\bin\\mvn.cmd" clean package'
            }
        }
    }
}
