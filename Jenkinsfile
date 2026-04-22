pipeline {
    agent any

    stages {

        stage('Clone') {
            steps {
                git 'https://github.com/sameera-8/ci-cd-demo.git'
            }
        }

        stage('Docker Build') {
            steps {
                sh 'docker build -t myapp .'
            }
        }

        stage('Run Container') {
            steps {
                sh 'docker run -d myapp'
            }
        }
    }
}
