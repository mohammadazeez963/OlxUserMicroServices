pipeline {
    agent any

    stages {
        stage('checkout') {
            steps {
                git 'https://github.com/mohammadazeez963/javaProject.git'
            }
        }
        stage('compile') {
            steps {
                bat 'mvn clean compile'
            }
        }
        stage('run') {
            steps {
                bat 'mvn package'
            }
        }
         stage('Test report using jacoco') {
            steps {
                echo 'jacoco'
            }
        }
        stage('Building Docker Image') {
            steps {
                echo 'Building Docker Image'
            }
        }
    }
}
