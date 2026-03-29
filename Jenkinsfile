pipeline {
    agent any

    stages {
        stage('Clone Code') {
            steps {
                git 'https://github.com/Tanishkaavats/Devopsrepo-exp8'
            }
        }

        stage('Build Image') {
            steps {
                sh 'docker build -t my-app .'
            }
        }

        stage('Run Container') {
            steps {
                sh 'docker run -d -p 3000:3000 my-app'
            }
        }
    }
}