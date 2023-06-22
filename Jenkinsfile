pipeline {
    agent any

    stages {
        stage('Maven Version Check') {
            steps {
                sh 'mvn --version'
            }
        }
        
        stage('Test the code') {
            steps {
                sh 'mvn clean test'
            }
        }
     
    }
}
