pipeline {
    agent {
        docker {
            image 'node:6-alpine' 
            args '-p 3000:3000' 
        }
    }
    stages {
        stage('Pull') {
            scm checkout
        }
        stage('Install Dependencies') { 
            steps {
		        sh 'npm --version'
                sh 'npm install'
            }
        }
    }
}
