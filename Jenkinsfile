pipeline {
    agent any
    stages {
        stage('ServersHealthCheck') {
            steps {
                sh 'ssh mercury@192.168.1.186'
                sh 'bash checkHealth'
            }
        }
    }
    post { 
        always { 
            echo 'All Servers Health Checks Done!'
        }
    }
}