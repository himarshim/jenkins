pipeline {
    agent any

    stages {
        stage('code checkout') {
            steps {
                checkout scmGit(branches: [[name: '*/master']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/himarshim/jenkins']])
            }
        }
    }
}

