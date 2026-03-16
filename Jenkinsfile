pipeline {
    agent any

    stages {

        stage('Pull from Git') {
            steps {
                git 'https://github.com/yourusername/jenkins-pipeline-demo.git'
            }
        }

        stage('Build') {
            steps {
                echo "Building the project..."
                sh 'python app.py'
            }
        }

        stage('Test') {
            steps {
                echo "Running tests..."
                sh 'pytest test_app.py'
            }
        }

        stage('Deploy') {
            steps {
                echo "Deploying application..."
                sh 'echo Deployment Successful'
            }
        }
    }
}
