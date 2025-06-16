pipeline {
    agent any

    stages {
        stage('Code Cloning...') {
            steps {
                git 'https://github.com/trivediayush/Notes-Keeping.git'
            }
        }

        stage('Building Image...') {
            steps {
                sh "docker build -t mydemoNotes ."
            }
        }
      
        stage('Pushing Image to DockerHub...') {
            steps {
                sh "docker images"
            }
        }
    }
}
