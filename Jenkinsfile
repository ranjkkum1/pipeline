pipeline {
    agent any
    stages {
    stage('code checkout') {
        steps {
            checkout([$class: 'GitSCM', branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[credentialsId: 'GitHub', url: 'git@github.com:ranjkkum1/pipeline.git']]])
        }
    }
        stage('build') {
            steps {
                sh 'date'
            }
        }
    }
}
