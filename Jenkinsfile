pipeline {
    agent any

    stages {

        stage('Clone') {
            steps {
                git 'https://github.com/deekshithar95/carwebsite.git'
            }
        }

        stage('Deploy') {
            steps {
                sh '''
                sudo rm -rf /var/www/html/*
                sudo cp -r * /var/www/html/
                '''
            }
        }
    }
}
