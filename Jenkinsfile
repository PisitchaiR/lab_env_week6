pipeline{
    agent any
    stages{
        stage("one"){
            environment {
                fname = 'kamal'
            }
            steps {
                sh 'echo "hello ${fname}"'
            }
        }
        stage("two") {
            steps {
                sh 'echo "hello ${fname}"'
            }
        }
    }
}