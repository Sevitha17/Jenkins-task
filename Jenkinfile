pipeline {
    agent any

    stages {

        stage('Clone Code') {
            steps {
                git 'https://github.com/Sevitha17/Jenkins-task.git'
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
                    sudo cp -r * /var/www/html/
                '''
            }
        }
    }
}
