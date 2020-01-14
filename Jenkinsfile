pipeline {
   /* agent any
    stages {
        stage('Build') {
            steps {
                sh 'echo "Hello world!"'
            }
        }
    }*/
    agent {
        docker {
            image 'node:latest' 
            args '-p 3000:3000' 
        }
    }
    stages {
        stage('Build') { 
            steps {
		sh 'docker ps'
                sh 'npm install' 
            }
        }
    }
}
