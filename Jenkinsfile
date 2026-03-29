pipeline {
    agent any

    stages {

        stage('Build Image') {
            steps {
                script {
                    docker.build("myapp")
                }
            }
        }

        stage('Run Container') {
            steps {
                script {
                    docker.run("myapp")
                }
            }
        }
    }
}