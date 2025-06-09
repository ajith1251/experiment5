pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                git 'https://github.com/ajith1251/experiment5.git'
            }
        }

        stage('Build') {
            steps {
                sh 'echo "Build step goes here"'
            }
        }

        stage('Test') {
            steps {
                sh 'echo "Test step goes here"'
            }
        }

        stage('Deploy') {
            steps {
                sh 'echo "Deploy step goes here"'
            }
        }
    }
}
