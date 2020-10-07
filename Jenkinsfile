pipeline {
    agent none
    stages {
        stage('Example Build') {
		
            steps {
			sh 'apt-get update -y'
			sh 'apt-get install -y maven'
            sh 'mvn --version'
            }
        }
    }
}