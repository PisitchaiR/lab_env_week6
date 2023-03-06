pipeline {
    agent any

    stages {
        stage("build") {
            steps {
                echo "Building"
                sh "python --version"
            }
        }
    }
    post {
        always {
            echo "Cleaning up"
        }
        failure {
            echo "Failed"
        }
    }
}