pipeline {
    agent any
    stages {
        stage('ServersHealthCheck') {
            steps {
                sh 'mercury'
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