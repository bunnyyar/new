pipeline {
    agent any 
    stages {
        stage('checkout') {
            steps {
                'https://github.com/bunnyyar/new.git'
            }
        }
        stage('build') {
            steps {
                sh 'npm install'
            }
        }
        stage('test') {
            steps {
                sh 'npm test'
            }
        }
        
    }
}
