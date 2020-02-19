pipeline {
    agent {
        docker {
            image 'node:13.8.0-alpine3.11' 
            args '-p 3000:3000' 
        }
    }
    stages {
        stage('Install Dependencies') { 
            steps {
		        sh 'npm --version'
                sh 'npm install'
            }
        }
    }
}
