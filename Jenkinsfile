pipeline {
    agent any

    environment {
        PYTHON = "python3"
    }

    stages {

        stage('Verify Environment') {
            steps {
                sh '''
                echo "OS:"
                uname -a

                echo "Python:"
                $PYTHON --version
                '''
            }
        }

        stage('Build') {
            steps {
                sh '''
                echo "Build stage"
                $PYTHON demo.py
                '''
            }
        }

        stage('Test') {
            steps {
                sh '''
                echo "Test stage"
                $PYTHON test.py
                '''
            }
        }

        stage('Deploy') {
            steps {
                sh '''
                echo "Deploy stage"
                $PYTHON demo1.py
                '''
            }
        }
    }

    post {
        failure {
            echo "❌ Pipeline failed — fix your scripts"
        }
        success {
            echo "✅ Pipeline completed successfully"
        }
    }
}
