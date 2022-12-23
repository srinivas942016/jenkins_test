properties([pipelineTriggers([githubPush()])])

pipeline {
    agent any
    
   

    stages {
        stage('Pullscm') {
            steps {
                // Get some code from a GitHub repository
                git credentialsId: 'github', url: 'git@github.com:srinivas942016/jenkins_test.git'
			}
		}
		
		stage('print') {
		    
		    steps {
		        sh "echo testing running a stage on node and git code pulled successfully"
		    }
		}
			
		
    }
}
