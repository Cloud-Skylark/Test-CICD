pipeline {
    agent { label 'Try-Node' }

    stages {
        stage('Clone Code') {
            steps {
                git url: 'https://github.com/Cloud-Skylark/Test-CICD.git', branch: 'main'
                echo 'Code cloned successfully'
            }
        }
        
        stage('Building') {
            steps {
                echo 'Building the project...'
            }
        }
        
        stage('Testing') {
            steps {
                echo 'Running tests...'
            }
        }

       stage('Deploy') {
            steps {
                sh 'sudo cp index.html /var/www/html/'
                echo 'Deployment successful to /var/www/html/'
            }
        }
    }
}
