pipeline {
    agent any
    stages {
        stage('git repo & clean') {
            steps {
              // bat "rmdir  /s /q fruteriasss"
                bat "git clone https://github.com/estudiante957/fruteriasss.git "
             
            }
        }
        stage('install') {
            steps {
                bat "npm install -f fruteriasss"
            }
        }
        stage('test') {
            steps {
                bat "npm test -f fruteriasss"
            }
        }
    }
}
