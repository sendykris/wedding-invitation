pipeline {
    agent {
        node {
            label "linux && java11"
        }
    }
    stages {
        
        stage("Create Nginx") {
            steps{
                sh 'docker run -d --restart unless-stopped nginx'
                sh 'docker ps -n 1'
                echo 'New Container Success Created'
            }
        }
    }
}