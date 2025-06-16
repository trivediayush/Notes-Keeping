pipeline {
    agent any

    triggers {
        githubPush()
    }

    stages {
        stage('Code Cloning...') {
            steps {
                git 'https://github.com/trivediayush/Notes-Keeping.git'
            }
        }

        stage('Building Image...') {
            steps {
                sh 'docker build -t mydemonotes .'
            }
        }

        stage('Pushing Image to DockerHub...') {
            steps {
                sh 'docker images'
            }
        }
    }
}
