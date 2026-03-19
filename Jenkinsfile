pipeline {
    agent any

    stages {
        stage('Clone Code') {
            steps {
                git 'https://github.com/YOUR-USERNAME/YOUR-REPO.git'
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