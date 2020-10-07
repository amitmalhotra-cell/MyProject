pipeline {
    agent {
                docker {
                  label 'dockerserver'  // both label and image
                  image 'maven:3-alpine'
                }
            }
    stages {
        stage('Example Build') {
            steps {
                sh 'mvn -B clean verify'
            }
        }
    }
}