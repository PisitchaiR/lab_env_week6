pipeline{
    agent any
    environment {
        GIT_CREDS = credentials('github')
    }
    stages {
        stage('abc'){
            steps{
                sh 'echo "Git user is $GIT_CREDS_USERNAME"'
                sh 'echo "Git password is $GIT_CREDS_PASSWORD"'
                sh 'echo "Current build number is $BUILD_NUMBER"'
            }
        }
    }
}