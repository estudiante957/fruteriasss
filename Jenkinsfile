pipeline {
    agent any
    stages {
        stage('git repo & clean') {
            steps {
               bat "rmdir  /s /q fruteriasss"
                bat "git clone "
                bat "mvn clean -f fruteriasss"
            }
        }
        stage('install') {
            steps {
                bat "mvn install -f fruteriasss"
            }
        }
        stage('test') {
            steps {
                bat "mvn test -f fruteriasss"
            }
        }
        stage('package') {
            steps {
                bat "mvn package -f fruteriasss"
            }
        }
    }
}