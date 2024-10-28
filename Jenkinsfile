pipeline {
    agent {
        node {
            label 'python'
        }
    }
    stages {
        stage('Test Docker Setup') {
            steps {
                script {
                    echo 'Testing Docker Setup'
                    sh 'python3 -m venv my-venv'
                    sh 'my-venv/bin/pip install pandas'
                }
            }
        }
    }
    post {
        always {
            echo 'Pipeline completed!'
        }
    }
}
