pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
            }
        }
        stage('npn test'){
            agent{
                docker{
                    image 'node:18-alpine'
                }
            }
            steps{
                sh 'npm --version'
            }
        }
    }
}
