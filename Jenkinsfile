pipeline{
    agent any
    parameters {
        string(name: 'NAME', defaultValue: 'Uthred', description: 'Entere your name')
        choice(name: 'CITY', choices: ['Bebbanburg', 'Mercia', 'East Anglia'], description: 'Choose your city')
    }
    stages {
        stage('Hello') {
            steps {
                echo "Hello ${params.NAME} from ${params.CITY}"
            }
        }
    }
}