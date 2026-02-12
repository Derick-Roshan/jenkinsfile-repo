pipeline {
    agent any 

    stages {

        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Build') { 
            steps {
                sh 'python3 demo.py'
            }
        }

        stage('Test') { 
            steps {
                sh 'python3 test.py'
            }
        }

        stage('Deploy') { 
            steps {
                sh 'python3 demo1.py'
            }
        }
    }
}
