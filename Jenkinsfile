pipeline {
    agent any

    stages {

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
