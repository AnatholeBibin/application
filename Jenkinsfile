pipeline {
    agent any 
    stages {
        stage('clone') { 
            steps {
                sh "rm -rf *"
                sh "git clone https://github.com/AnatholeBibin/application/blob/master/"
            }
        }
        stage('build') { 
            steps {
                sh "cd application/blob/master/ && javac Main.java"
            }
        }
        stage('run') { 
            steps {
                sh "cd application/blob/master/ && java Main"
            }
        }
    }
}
