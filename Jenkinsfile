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
                bat 'py app.py'
            }
        }

        stage('Test') {
            steps {
                bat 'py -m pytest test_app.py'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deployment Successful'
            }
        }
    }
}
