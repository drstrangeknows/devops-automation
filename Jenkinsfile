pipeline {
    agent any
    stages{
        stage('Build Maven'){
            steps{
                checkout([$class: 'GitSCM', branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/drstrangeknows/devops-automation.git']]])
                sh 'mvn clean install'
            }
        }
    }
}
