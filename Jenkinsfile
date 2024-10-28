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
                    sh 'pip install pandas'
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
