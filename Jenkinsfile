pipeline {
    agent { label 'Try-Node' }

    stages {
        stage('Clone Code') {
            steps {
                git url: 'https://github.com/YOUR-USERNAME/YOUR-REPO.git', branch: 'main
                echo 'code succefull'
            }
        }
        stage('Building') {
            steps {
                echo 'code building'
            }
        }
        stage('Testing') {
            steps {
                echo 'code testing'
            }
        }

        stage('Deploy') {
            steps {
                sh 'cp index.html /var/www/html/'
            }
        }
    }
}
