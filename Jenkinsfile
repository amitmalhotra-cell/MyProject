pipeline {
    agent none
    stages {
        stage('Example Build') {
		agent {
                docker { image 'maven:3-alpine' }
            }
            steps {
                sh 'mvn --version'
            }
        }
    }
}