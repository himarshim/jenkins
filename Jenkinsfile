pipeline {
    agent any

    stages {
        stage('code checkout') {
            steps {
                checkout scmGit(branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/himarshim/jenkins']])
            }   
        }     
        stage('code checkout') {
            steps {
                sh 'aws s3 ls'
            }
        }
        
    }
}

