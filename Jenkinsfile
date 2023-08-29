pipeline {
    agent any 
    stages {
        stage('clone') { 
            steps {
                sh "rm -rf *"
                sh "git clone https://github.com/AnatholeBibin/application"
            }
        }
        stage('build') { 
            steps {
                sh "cd application/ && javac Main.java"
            }
        }
        stage('run') { 
            steps {
                sh "cd application/ && java Main"
            }
        }
    }
}
