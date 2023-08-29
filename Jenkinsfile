pipeline {
    agent any 
    stages {
        stage('clone') { 
            steps {
                sh "rm -rf *"
                sh "git clone https://github.com/AnatholeBibin/expose.git"
            }
        }
        stage('build') { 
            steps {
                sh "cd expose/ && javac Main.java"
            }
        }
        stage('run') { 
            steps {
                sh "cd expose/ && java Main"
            }
        }
    }
}
