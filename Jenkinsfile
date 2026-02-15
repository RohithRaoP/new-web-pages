pipeline {
    agent any

    triggers {
// polls the scm every 1 minute
        pollSCM('h/1 * * * *')
    }

    stages {

        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Build') {
            steps {
                echo "checked for changes if any happped  Builded it "
                sh 'ls -la'
                echo "Build completed successfully!"
            }
        }

    }
}
