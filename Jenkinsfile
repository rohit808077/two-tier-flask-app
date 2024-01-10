pipeline {
    agent  none
    
    stages{
        }
        stage("Build & Test"){

		agent {
                label 'stag-server'
            }

            steps{
                sh "docker build -t two-tier-falsk-app ."
            }
        }
       
    }
}
