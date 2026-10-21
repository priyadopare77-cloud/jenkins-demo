pipeline {
    agent any

    stages {
        stage('Run App') {
            steps {
                sh 'python3 app.py'
            }
        }

        stage('Build Docker') {
            steps {
                sh 'docker build -t hello-jenkins .'
            }
        }
    }
}
