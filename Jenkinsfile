pipeline {
    agent {
        docker {
            image 'nginx'
            args '-p 3000:80'
        }
    }
    stages {
        stage('Build') {
            steps {
                echo "Built"
            }
        }
        stage('Deliver') { 
            steps { 
                input message: 'Finished using the web site? (Click "Proceed" to continue)' 
            }
        }
    }
}
