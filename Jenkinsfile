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
                bat 'python demo.py'
            }
        }

        stage('Test') { 
            steps {
                bat 'python test.py'
            }
        }

        stage('Deploy') { 
            steps {
                bat 'python demo1.py'
            }
        }
    }
}
