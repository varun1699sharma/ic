pipeline {
    agent any
    stages {
        stage('git repo & clean') {
            steps {
                //bat "rmdir  /s /q ic"
                bat "git clone https://github.com/varun1699sharma/ic.git"
                bat "mvn clean"
            }
        }
        stage('install') {
            steps {
                bat "mvn install"
            }
        }
   
        stage('package') {
            steps {
                bat "mvn package"
            }
        }
    }
}
