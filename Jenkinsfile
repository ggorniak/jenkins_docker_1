pipeline {
    agent any
        environment {
            python="'C:\Users\Student\Python\Python313\python.exe'"
        }
    stages {
        stage('Build') {
            steps {
                bat "${python} new_file.py"
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
