pipeline {
    agent any 
    stages {
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








// how to run the python file form the jenkins file
// sh 'python3 your_script.py' 

