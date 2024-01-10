pipeline {
    agent  none
    
    stages{
        stage("Code"){

		agent {
                label 'dev-server'
            }

            steps{
                git url: "https://github.com/rohit808077/two-tier-flask-app.git", branch: "master"
            }
        }
        stage("Build & Test"){

		agent {
                label 'stage-server'
            }

            steps{
                sh "docker build -t two-tier-falsk-app ."
            }
        }
       
    }
}
