pipeline {
    agent {
        docker {
            image 'nginx'
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
