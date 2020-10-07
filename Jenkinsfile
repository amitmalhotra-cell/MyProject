pipeline {
    agent any
    stages {
        stage('Example Build') {
		
            steps {
			sh 'chmod 0700 /var'
			sh 'apt-get update && apt-get install -y maven'
			sh 'mvn --version'
            }
        }
    }
}