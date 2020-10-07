pipeline {
    agent {
    docker {
        image 'maven:3-alpine'
        label 'docker'
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