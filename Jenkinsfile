pipeline {
    agent any
    stages {
        stage('Create Image') {
            steps {
                sh 'docker build . -t hello-app'
            }
        }
        stage('Create a container') {
            steps {
                sh 'docker run -p 4000:3000 -d hello-app'
            }
        }
    }
}
