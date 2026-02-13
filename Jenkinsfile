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
                bat "C:/Users/ROSHAN/AppData/Local/Programs/Python/Python314/python.exe test.py"

            }
        }

        stage('Test') { 
            steps {
                bat "C:/Users/ROSHAN/AppData/Local/Programs/Python/Python314/python.exe test.py"

            }
        }

        stage('Deploy') { 
            steps {
                bat "C:/Users/ROSHAN/AppData/Local/Programs/Python/Python314/python.exe demo1.py"

            }
        }
    }
}
