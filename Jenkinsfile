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
                bat '"C:\\Users\\Aditya Rana\\AppData\\Local\\Programs\\Python\\Python313\\python.exe" app.py'
            }
        }

        stage('Test') {
            steps {
                bat '"C:\\Users\\Aditya Rana\\AppData\\Local\\Programs\\Python\\Python313\\python.exe" -m pytest test_app.py'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deployment Successful'
            }
        }
    }
}
