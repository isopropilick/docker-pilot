pipeline {
    agent {
        node {
            label 'node'
        }
    }
    stages {
        stage('Test Docker Setup') {
            steps {
                script {
                    echo 'Testing Docker Setup'
                    sh 'npm -v'
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
