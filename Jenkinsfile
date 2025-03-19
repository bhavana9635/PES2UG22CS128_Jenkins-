pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                script {
                    sh 'g++ -o PES2UG22CS128-1 hello.cpp'
                }
            }
        }

        stage('Test') {
            steps {
                script {
                    sh './PES2UG22CS128-1'
                }
            }
        }

        stage('Deploy') {
            steps {
                echo "Deploy step - Add actual deployment commands here"
            }
        }
    }

    post {
        failure {
            echo "Pipeline failed!"
        }
    }
}
