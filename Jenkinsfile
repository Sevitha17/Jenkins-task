pipeline {
    agent any

    stages {

        stage('Clone Code') {
            steps {
                git branch: 'main',
                    url: 'https://github.com/Sevitha17/Jenkins-task.git'
            }
        }

        stage('Build') {
            steps {
                echo "No build required for static website"
            }
        }

        stage('Deploy') {
            steps {
                sh '''
                    cp -r index.html style.css /var/www/html/
                '''
            }
        }
    }
}
