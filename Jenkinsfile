
pipeline {
    agent any 
    stages {
        stage('Build Environment') { 
            steps {
                echo "Build python"
                sh '''  python3.5 -v
                        virtualenv venv
                        . ./venv/bin/activate
                        cd webapp
                        pip install -r requirements.txt
                   '''
            }
        }
        stage('Test') { 
            steps {
                echo "Test"
                sh '''
                        pip list
                        python webapp/tests.py
                '''
            }
        }
        stage('Deploy') { 
            steps {
                echo "Deploy"
            }
        }
    }
}
