pipeline {
    agent any 
    stages {
        stage('clone') { 
            steps {
                sh "rm -rf *"
                sh "git clone https://github.com/AnatholeBibin/application.git"
            }
        }
        stage('build') { 
            steps {
                sh "cd application.git/ && javac main.java"
            }
        }
        stage('run') { 
            steps {
                sh "cd application.git/ && java main"
            }
        }
    }
}
