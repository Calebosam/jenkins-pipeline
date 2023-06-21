pipeline{
    agent{
        label "jenkins-node-python-agent"
    }
    stages{
        stage("Testing"){
            steps{
                sh "node server.js"
            }
        }
    }
}