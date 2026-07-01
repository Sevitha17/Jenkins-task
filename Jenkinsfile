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
                echo 'Frontend build completed'
            }
        }

        stage('Deploy') {
            steps {
                sh '''
                    mkdir -p deploy
                    cp index.html style.css deploy/
                '''
            }
        }
    }
}
