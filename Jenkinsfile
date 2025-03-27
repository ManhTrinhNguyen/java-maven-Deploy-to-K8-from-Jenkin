#!/usr/bin/env groovy

pipeline {
    agent any

    environment {
        PROJECT_NAME = "MySampleProject"
    }

    stages {
        stage('Checkout') {
            steps {
                echo "Cloning the repo."
                checkout scm
            }
        }

        stage('Build') {
            steps {
                echo "Building ${env.PROJECT_NAME}"
                // Simulate a build step
                sh 'echo Build complete!!!!!'
            }
        }

        stage('Test') {
            steps {
                echo "Running tests..."
                // Simulate tests
                sh 'echo All tests passed!'
            }
        }

        stage('Deploy') {
            steps {
                echo "Deploying ${env.PROJECT_NAME}..."
                // Simulate deployment
                sh 'echo Deployed successfully!'
            }
        }
    }

    post {
        success {
            echo "Pipeline completed successfully!"
        }
        failure {
            echo "Pipeline failed!"
        }
    }
}
