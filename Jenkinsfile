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
                echo 'Pulling...';
                git branch :'main',
                url:'https://github.com/Outayel/DevopsTest.git';
            }
        }
          stage('MVN') {
            steps {
                 sh """mvn -version"""
            }
        }
         stage('MVN clean') {
            steps {
                 sh "mvn clean install"
            }
        }
    }
}
