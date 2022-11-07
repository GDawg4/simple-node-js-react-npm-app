pipeline {
    agent {
        docker {
            image 'nginx'
            args '-p 80:3000'
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
