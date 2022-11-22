pipeline {
    agent any
    stages {
        stage('git repo & clean') {
            steps {
              // bat "rmdir  /s /q fruteriasss"
                bat "git clone https://github.com/estudiante957/fruteriasss.git "
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
    }
}
