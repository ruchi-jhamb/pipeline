pipeline {
    agrnt any;
    stages {
        stage('Set Up') {
            CleanWs();
            steps {
                CleanWs();
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
