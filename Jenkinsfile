pipeline {
    agent any

    stages {
        stage('code checkout') {
            steps {
                checkout scmGit(branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/himarshim/jenkins']])
            }   
        }     
        stage('S3 List') {
            steps {
                sh 'aws s3 ls'
            }
        }
        
    }
}

