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
        stage('Build') {
            steps {
                bat "Building -f fruteriasss"
            }
        }
        stage('Test') {
            steps {
                bat "Testing -f fruteriasss"
            }
        }
    }
}
