
pipeline {
    agent any 
    stages {
        stage('Build') { 
            steps {
                echo "Build python"
                sh '''  python3.5 -v
                        virtualenv venv
                   '''
            }
        }
        stage('Test') { 
            steps {
                echo "Test"
            }
        }
        stage('Deploy') { 
            steps {
                echo "Deploy"
            }
        }
    }
}
