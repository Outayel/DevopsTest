pipeline {
    agent any
    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
            }
        }
          stage('Git') {
            steps {
                echo 'Pulling... Latest';
            }
        }
          stage('MVN') {
            steps {
                 sh """mvn -version"""
            }
        }
         stage('MVN Complie') {
            steps {
                 sh """mvn compile"""
            }
        }
         stage('MVN clean') {
            steps {
                 sh """mvn clean"""
            }
        }
    }
}
