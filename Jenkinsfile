pipeline {
    agent any
    stages {
        stage('ServersHealthCheck') {
            steps {
                sh './checkHealth'
            }
        }
    }
    post { 
        always { 
            echo 'All Servers Health Checks Done!'
        }
    }
}