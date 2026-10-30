pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo 'Source code checkout stage'
            }
        }

        stage('Build') {
            steps {
                echo 'Build stage started'
                sh 'echo "Application build successful"'
            }
        }

        stage('Test') {
            steps {
                echo 'Test stage started'
                sh 'echo "Application tests successful"'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploy stage started'
                sh 'echo "Deployment stage completed"'
            }
        }
    }

    post {
        success {
            echo 'Pipeline completed successfully'
        }

        failure {
            echo 'Pipeline failed'
        }
    }
}
