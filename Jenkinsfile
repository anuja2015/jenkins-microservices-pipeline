pipeline {
    //agent any
    agent { 
        docker { 
            image 'maven:3.6.3' 
        } 
    }

    stages {
      //  stage('Preparation') { // for display purposes
        //    steps{
          //      checkout([$class: 'GitSCM', branches: [[name: '*/master']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/anuja2015/jenkins-microservices-pipeline.git']]])
            
            //}
        //}
        stage('Build') {
            steps{
                sh 'mvn --version'
            }
        }
        stage('Results') {
            steps{
                echo "docker image used as a jenkins agent"
            }
        }
    }
    post{
        success{
            echo "Success"
        }
        failure{
            echo "Failure"
        }
    }
}