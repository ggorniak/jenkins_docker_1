pipeline {
    agent any
        environment {
            python='"C:\\Users\\Student\\Python\\Python313\\python.exe"'
        }
    stages {
        stage('Build') {
            steps {
                bat "${python} new_file.py"
            }
        }
        stage('Parallel Tasks') {
          steps {
            parallel(
              a: {
                echo "This is branch a"
              },
              b: {
                echo "This is branch b"
              }
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
