pipeline {
    agent any

    triggers {
        githubPush()
    }

    stages {

        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Build') {
            steps {
                echo "New change detected. Starting build..."
                sh 'ls -la'
                echo "Build completed successfully!"
            }
        }

    }
}
