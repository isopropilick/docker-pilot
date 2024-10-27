pipeline {
    agent any
    stages {
        stage('Test Docker Setup') {
            steps {
                script {
                    echo 'Testing Docker Setup'
                    sh 'echo "Docker is running properly inside Jenkins!"'
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
