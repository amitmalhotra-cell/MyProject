pipeline {
    agent any
    stages {
	    stage('Quality Gate status check'){
		    steps{
			    script{
				    withSonarQubeEnv('sonarserver'){
				    sh "mvn sonar:sonar"
				    }
				    timeout(time:1,unit:'HOURS'){
				    def qg=waitForQualityQate()
					    if(qg.status!='OK'){
						    error "pipeline aborted due to quality gate failure : ${qg.status}"
					    }
				    }
				    sh "mvn clean install"
			    
			    }
		    }
	    }
    }
}
