pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..PDV'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..PDV'
                sh label: 'API Collection Tests', script: 'newman run PDV.postman_collection.json --suppress-exit-code'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....PDV'
            }
        }
    }
}
