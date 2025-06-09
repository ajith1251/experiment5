pipeline {
    agent any

    environment {
        REPO_URL = 'https://github.com/ajith1251/experiment5.git'
        BRANCH = 'main'
    }

    stages {
        stage('Clone') {
            steps {
                git branch: "${BRANCH}", url: "${REPO_URL}"
            }
        }

        stage('Build') {
            steps {
                echo 'Running build...'
                // put your build commands here (e.g. compile, npm install, etc.)
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests...'
                // put your test commands here
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying app...'
                sh 'nohup python3 -m http.server 8000 &'
            }
        }
    }
}


