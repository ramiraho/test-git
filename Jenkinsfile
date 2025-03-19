pipeline {
    agent any

    stages {
        // Stage 1: Checkout Code
        stage('Checkout') {
            steps {
                echo 'Checking out code from Git...'
                git branch: 'main', url: 'https://github.com/ramiraho/test-git.git'
            }
        }

        // Stage 2: Build
        stage('Build') {
            steps {
                echo 'Building the application...'
                //sh './build.sh' // Replace with your build command
            }
        }

        // Stage 3: Test
        stage('Test') {
            steps {
                echo 'Running tests...'
                //sh './test.sh' // Replace with your test command
            }
        }

        // Stage 4: Deploy
        stage('Deploy') {
            steps {
                echo 'Deploying the application...'
                //sh './deploy.sh' // Replace with your deploy command
            }
        }
    }

    post {
        success {
            echo 'Pipeline succeeded!'
        }
        failure {
            echo 'Pipeline failed!'
        }
    }
}