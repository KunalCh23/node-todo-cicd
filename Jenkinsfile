pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh "docker build . -t myimg"
                sh "docker run -d --name node-cont -p 8000:8000 myimg"
            }
        }
    }
}
