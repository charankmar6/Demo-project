pipeline {
    agent any
    }
    stages{
        stage('Build Maven'){
            steps{
                checkout([$class: 'GitSCM', branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/charankmar6/Demo-project']]])
                sh 'mvn clean install'

                }
            }
        }
    }