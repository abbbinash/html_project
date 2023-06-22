pipeline {
    agent any

    stages {
        stage('Maven Version Check') {
            steps {
                sh 'mvn --version'
            }
        }
        stage('Build the project'){
            steps {
                sh *jar -cvf test.war *'
            }
        }
        stage('Test the code') {
            steps {
                sh 'mvn clean tets'
            }
        }
     
    }
}
