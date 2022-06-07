pipeline {
    agent any

    stages {
        
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
                jacoco()
            }
        }
        stage('Building Docker Image') {
            steps {
                echo 'Building Docker Image'
            }
        }
    }
}
