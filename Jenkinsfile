pipeline {
    agent any 

    tools Nodejs {'nodejs'
    }
    stages {
        stage('checkout') {
            steps {
               git credentialsId: '6a466836-8697-41a3-b2ae-06c69062b2bf', url: 'https://github.com/bunnyyar/new'
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
