pipeline {
    agent {
        docker {
            image 'node:6-alpine' 
            args '-p 3000:3000' 
        }
    }
    echo "Running ${env.BUILD_ID} on ${env.JENKINS_URL}"
    stages {
        stage('Install Dependencies') { 
            steps {
		        sh 'npm --version'
                sh 'npm install'
            }
        }
    }
}
