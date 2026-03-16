pipeline {
    agent any

    stages {

        stage('Pull from Git') {
            steps {
                echo 'Repository already checked out'
            }
        }

        stage('Build') {
            steps {
                bat 'python app.py'
            }
        }

        stage('Test') {
            steps {
                bat 'pytest test_app.py'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deployment successful'
            }
        }
    }
}
