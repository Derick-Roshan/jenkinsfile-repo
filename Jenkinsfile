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
                bat bat "\"C:/Users/ROSHAN/AppData/Local/Programs/Python/Python314/python.exe\" demo.py"

            }
        }

        stage('Test') { 
            steps {
                bat bat "\"C:/Users/ROSHAN/AppData/Local/Programs/Python/Python314/python.exe\" test.py"

            }
        }

        stage('Deploy') { 
            steps {
                bat bat "\"C:/Users/ROSHAN/AppData/Local/Programs/Python/Python314/python.exe\" demo.py"

            }
        }
    }
}
