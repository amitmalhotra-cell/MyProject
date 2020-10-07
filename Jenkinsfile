pipeline {
    agent { label 'dockerserver' }
    stages {
        stage('Example Build') {
		agent {
                docker {
                  label 'dockerserver'  // both label and image
                  image 'maven:3-alpine'
                }
            }
            steps {
                sh 'mvn -B clean verify'
            }
        }
    }
}