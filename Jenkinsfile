pipeline {
    agent any

    stages {
        stage("pre -build") {
            steps {
                sh 'echo Pre-build'
            }
        }
        stage ("test") {
            steps {
                sh "echo Build in progress"
            }
        }
        stage ("Unit tests")
        {
            steps {
                sh "echo Unit tests"
            }
        }
        stage('deploy')
        {
            steps {
                sh "echo Deploy"
            }
        }
        stage('Regression tests')
        {
            steps {
                parallel{
                    stage('chrome'){
                        steps{
                            bat "echo chrome"
                        }
                    }
                    stage('safari'){
                        steps{
                            bat "echo chrome"
                        }
                    }
                }
            }
        }
        stage('Release to production')
        {
            steps {
                sh "echo Release to production"
            }
        }
    }
    post {
        always {
            echo "Always"
        }
        success{
            echo "Success"
        }
        failure {
            echo "Failed"
        }
        unstable {
            echo "Unstable"
        }
        changed {
            echo "Changed"
        }
    }
}