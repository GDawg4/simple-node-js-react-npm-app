pipeline {
    agent {
        docker {
            image 'nginx'
            args '-p 3000:3000'
        }
    }
    stages {
        stage('Build') {
            steps {
                sh 'npm install'
            }
        }
        stage('Deliver') { 
            steps { 
                input message: 'Finished using the web site? (Click "Proceed" to continue)' 
            }
        }
    }
}
