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
                    sh 'python3 -m venv ./venv'
                    sh 'source ./venv/bin/activate'
                    sh 'pip3 install pandas'
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
