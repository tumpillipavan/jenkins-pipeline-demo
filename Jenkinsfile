pipeline {
    agent any

    environment {
        MY_VAR = "Hello from Jenkins Environment"
    }

    stages {
        stage('Clone Repository') {
            steps {
                echo 'Repository will be cloned by Jenkins when job starts...'
            }
        }

        stage('Run Shell Script') {
            steps {
                sh './myscript.sh'
            }
        }

        stage('Print Working Directory') {
            steps {
                sh 'pwd'
            }
        }

        stage('Print Environment Variable') {
            steps {
                echo "The environment variable is: ${env.MY_VAR}"
            }
        }
    }
}
