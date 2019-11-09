
pipeline {
    agent any 
    stages {
        stage('Build Environment') { 
            steps {
                echo "Build python"
                bash '''  python3.5 -v
                        virtualenv venv
                        source venv/bin/activate
                        cd webapp
                        pip install -r requirements.txt
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
