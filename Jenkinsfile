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
                bat "/usr/bin/python3 test.py"

            }
        }

        stage('Test') { 
            steps {
                bat "/usr/bin/python3 test.py"

            }
        }

        stage('Deploy') { 
            steps {
                bat "/usr/bin/python3 demo1.py"

            }
        }
    }
}
