pipeline {
    agent any
    tools {
    
    jdk 'jdk17'
        maven 'maven3'
    }
    
    stages {  
        stage('Compiling') {
            steps {
            sh 'mvn compile'
            }
        }
        
        stage('Test') {
            steps {
                sh 'mvn test'
            }
        }
        
        stage('Build') {
            steps {
                sh 'mvn package'
            }
        }
    }
}
