
pipeline {
    agent any

    stages {
        stage('Build Docker') {
            steps {
                sh 'docker build -t hello-jenkins .'
                sh 'docker rm -f hello-jenkins || true'
                sh 'docker run -d --name hello-jenkins -p 8081:8080 hello-jenkins'
            }
        }
    }
}
