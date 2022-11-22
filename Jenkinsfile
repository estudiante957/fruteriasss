pipeline {
    agent any
    
    tools {nodejs "Node"}
    stages {
        stage('git') {
            steps {
              // bat "rmdir  /s /q fruteriasss"
                bat "git clone https://github.com/estudiante957/fruteriasss.git "
                
            }
        }
        stage('Build') {
            steps {
                bat "npm install"
            }
        }
        stage('Test') {
            steps {
                bat "Node test"
            }
        }
    }
}
