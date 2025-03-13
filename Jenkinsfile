pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                script {
                    sh 'g++ -o PES2UG22CS355-1 hello.cpp' // Compile main.cpp
                }
            }
        }

        stage('Test') {
            steps {
                script {
                    sh './PES2UG22CS355' // Run compiled output
                }
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying application' // Simulate deployment
            }
        }
    }

    post {
        failure {
            echo 'Pipeline failed'
        }
    }
}
