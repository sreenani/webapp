
pipeline {
    agent any 
    stages {
        stage('Build') { 
            steps {
                echo "Build python"
                python3 -v
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
