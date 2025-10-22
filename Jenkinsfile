pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                git url: 'https://github.com/neowyjr/Jenkins.git', branch: 'main'
            }
        }
        stage('Install') {
            steps {
                bat 'D:\\Python\\Python38\\Scripts\\pip install -r requirements.txt'
            }
        }
        stage('Test') {
            steps {
                bat 'D:\\Python\\Python38\\Scripts\\pytest'
            }
        }
    }
}
