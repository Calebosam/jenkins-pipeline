pipeline{
    agent{
        label "jenkins-node-python-agent"
    }
    environment{
        // PORT = 3000
        PORT = credentials("PORT")
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