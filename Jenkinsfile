pipeline {
    agent any

    stages {
        stage('Preparation') { // for display purposes
            steps{
                checkout([$class: 'GitSCM', branches: [[name: '*/master']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/anuja2015/jenkins-microservices-pipeline.git']]])
            
            }
        }
        stage('Build') {
            steps{
                sh 'pwd'
            }
        }
        stage('Results') {
            steps{
                echo "pipeline success"
            }
        }
    }
}