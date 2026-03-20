pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git branch: 'develop', url: 'https://github.com/Shivam-1022/my-project.git'
            }
        }

        stage('Build') {
            steps {
                echo "Building application..."
            }
        }

        stage('Test') {
            steps {
                echo "Testing application..."
            }
        }

        

        stage('Deploy') {
            steps {
                sh '''
                cp Jenkinsfile /var/www/html/
                '''
            }
        }
    }
}