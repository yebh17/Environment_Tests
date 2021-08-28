pipeline {
    agent any
    stages {
        stage('ServersHealthCheck') {
            steps {
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