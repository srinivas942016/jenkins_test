properties([pipelineTriggers([githubPush()])])

pipeline {
    agent any
    
    tools {
        // Install the Maven version configured as "M3" and add it to the path.
        maven "MVN3"
		jdk "jdk8"
    }

    stages {
        stage('Pullscm') {
            steps {
                // Get some code from a GitHub repository
                git credentialsId: 'github', url: 'git@github.com:srinivas942016/jenkins_test.git'
			}
		}
		
		stage('print') {
		    
		    steps {
		        sh "echo testing running a stage on node"
		    }
		}
			
		
    }
}
