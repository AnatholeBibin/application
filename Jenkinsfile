pipeline {
    agent any 
    stages {
        stage('clone') { 
            steps {
                sh "rm -rf *"
                sh "git clone https://github.com/priximmo/jenkins-helloworld"
            }
        }
        stage('build') { 
            steps {
                sh "cd jenkins-helloworld/ && javac main.java"
            }
        }
        stage('run') { 
            steps {
                sh "cd jenkins-helloworld/ && java main"
            }
        }
    }
}
