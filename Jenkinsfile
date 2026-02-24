pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                echo 'Cloning repository...'
            }
        }

        stage('Compile') {
            steps {
                bat 'javac Hello.java'
            }
        }

        stage('Run') {
            steps {
                bat 'java Hello'
            }
        }
    }

    post {
        success {
            echo 'Pipeline executed successfully ✅'
        }
        failure {
            echo 'Pipeline failed ❌'
        }
    }
}