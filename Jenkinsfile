pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/akashsakore/blue-ocean-jenkins.git'
            }
        }

        stage('Install') {
            steps {
                sh 'pip install pytest'
            }
        }

        stage('Test') {
            steps {
                sh 'pytest test_app.py'
            }
        }
    }
}

