pipeline {
    agent any;
    stages {
        stage('Set Up') {
          
            steps {
                cleanWs();
                sh 'echo setting up my workspace'
            }
        }

        stage('Checkout SCM'){
            steps {
                checkout scm
            }
        }
        stage('Compile Code') {
            steps{
                sh 'chmod +X app.sh'
            }
        }

        stage('Testing'){
            steps{
                sh 'sh app.sh'
            }
        }

    }
}
