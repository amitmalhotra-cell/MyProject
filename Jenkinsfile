pipeline {
    agent any
    stages {
        stage('Example Build') {
		
            steps {
			sh 'apt-get update && apt-get install -y maven'
			sh 'mvn --version'
            }
        }
    }
}