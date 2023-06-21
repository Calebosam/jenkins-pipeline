pipeline{
    agent{
        label "jenkins-node-python-agent"
    }
    environment{
        PORT = 3000
    }
    stages{
        stage("Install Dependencies"){
            steps{
                sh "npm install"
            }
        }

        stage("Run Applicaiton"){
            steps{
                sh "node server.js"
            }
        }
    }
}