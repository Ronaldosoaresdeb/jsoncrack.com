pipeline {
    agent any

    stages {
        stage('Git Checkout') {
            steps {
                checkout([$class: 'GitSCM', branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[credentialsId: '2de5b3be-ad42-4b1a-9e21-05c78c7104d3', url: 'https://github.com/Ronaldosoaresdeb/jsoncrack.com.git']]])
            }
        }
        stage('Build docker image'){
            steps{
                script{
                    sh 'docker build -t jsoncrack .'
                }
            }
        }

        
    }
}

